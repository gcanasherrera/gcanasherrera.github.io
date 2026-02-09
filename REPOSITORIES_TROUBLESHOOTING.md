# Repository Page Troubleshooting

## Issue: Repository cards not loading / showing broken images

**Symptom:** The repositories page looks broken, with missing or failed-to-load images where repository cards should appear.

**Cause:** The repository page uses external services (primarily `github-readme-stats.vercel.app`) to generate dynamic repository cards and statistics. These services are free, third-party hosted, and can experience:
- Rate limiting
- Temporary downtime
- Service interruptions

This is **not a bug in al-folio** but a limitation of the external services. See:
- [al-folio Issue #3388](https://github.com/alshedivat/al-folio/issues/3388)
- [github-readme-stats Issue #3851](https://github.com/anuraghazra/github-readme-stats/issues/3851)

## Solutions

### Option 1: Deploy Your Own Instance (Recommended)

The best long-term solution is to deploy your own instance of these services. It's free and takes about 10-15 minutes.

#### For github-readme-stats:

1. **Fork the repository:**
   - Visit [github-readme-stats](https://github.com/anuraghazra/github-readme-stats)
   - Click "Fork" in the top right

2. **Deploy to Vercel (free):**
   - Go to [Vercel](https://vercel.com/)
   - Sign in with your GitHub account
   - Click "New Project"
   - Import your forked `github-readme-stats` repository
   - Follow the deployment wizard (accept all defaults)
   - Note your deployment URL (e.g., `https://github-readme-stats-yourname.vercel.app`)

3. **Update your site configuration:**
   - Open `_config.yml` in your repository
   - Find the `external_services` section
   - Update the URL:
   
   ```yaml
   external_services:
     github_readme_stats_url: https://github-readme-stats-yourname.vercel.app
     github_profile_trophy_url: https://github-profile-trophy.vercel.app
   ```

4. **Commit and push changes:**
   ```bash
   git add _config.yml
   git commit -m "config: Use self-hosted github-readme-stats instance"
   git push
   ```

Your repository cards should now load reliably using your own instance!

#### For github-profile-trophy (optional):

If you also want to host the trophy service:

1. Fork [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy)
2. Deploy to Vercel (same process as above)
3. Update `github_profile_trophy_url` in `_config.yml`

See: [Deployment guide](https://github.com/ryo-ma/github-profile-trophy/issues/383)

### Option 2: Temporarily Disable Repository Page Features

If you don't want to deploy your own instance, you can disable specific features:

**Disable trophies** (in `_config.yml`):
```yaml
repo_trophies:
  enabled: false  # Change from true to false
```

**Disable the entire repositories page:**
- Delete or rename `_pages/repositories.md`
- Or remove it from navigation by setting `nav: false` in its frontmatter

### Option 3: Wait for Service Recovery

The default `github-readme-stats.vercel.app` service may recover after some time. However, this is not reliable for production sites.

## Checking if Services are Working

You can manually test if the services are accessible:

**Test github-readme-stats:**
```
https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME
```

**Test github-profile-trophy:**
```
https://github-profile-trophy.vercel.app/?username=YOUR_GITHUB_USERNAME
```

Open these URLs in your browser. If they load images, the service is working. If they show errors or timeout, the service is down.

## Related Documentation

- [CUSTOMIZE.md § Repository Page](CUSTOMIZE.md#repository-page-external-services) - Configuring external services
- [al-folio Issue #3388](https://github.com/alshedivat/al-folio/issues/3388) - Discussion about this issue
- [github-readme-stats documentation](https://github.com/anuraghazra/github-readme-stats) - Upstream project
- [github-profile-trophy documentation](https://github.com/ryo-ma/github-profile-trophy) - Trophy service

## Need Help?

- Check [GitHub Discussions](https://github.com/alshedivat/al-folio/discussions)
- Search [existing issues](https://github.com/alshedivat/al-folio/issues)
- Review the [FAQ](FAQ.md) and [TROUBLESHOOTING](TROUBLESHOOTING.md)
