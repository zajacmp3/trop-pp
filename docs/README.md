# TROP Privacy Policy - GitHub Pages Setup

This directory contains the privacy policy for TROP (Tactical Reconnaissance Operations Platform) hosted on GitHub Pages.

## Files

- `privacy-policy.html` - The main privacy policy page (styled HTML)
- `privacy-policy.md` - Privacy policy in Markdown format (for reference)
- `index.html` - Landing page that redirects to the privacy policy
- `_config.yml` - Jekyll configuration for GitHub Pages
- `README.md` - This file

## Setup Instructions

### Step 1: Enable GitHub Pages

1. Go to your GitHub repository settings
2. Navigate to **Settings** > **Pages**
3. Under **Source**, select:
   - Branch: `master` (or `feat/fastlane-api-35` if you want to use the current branch)
   - Folder: `/docs`
4. Click **Save**

### Step 2: Wait for Deployment

GitHub Pages will automatically build and deploy your site. This typically takes 1-2 minutes.

### Step 3: Access Your Privacy Policy

Your privacy policy will be available at:
```
https://<your-github-username>.github.io/<repository-name>/
```

Or directly at:
```
https://<your-github-username>.github.io/<repository-name>/privacy-policy.html
```

### Step 4: Update Configuration

Edit `_config.yml` and update the following:
```yaml
url: "https://<your-github-username>.github.io"
baseurl: "/<repository-name>"
```

### Step 5: Contact Information

The privacy policy has been configured with DefenceBay's contact information:
- Email: biuro@mzeds.pl
- Website: https://mzeds.pl

## For Google Play Store

When submitting your app to Google Play Store:

1. Use the privacy policy URL in your Play Store listing:
   ```
   https://<your-username>.github.io/<repository>/privacy-policy.html
   ```

2. Add the privacy policy link in the "Privacy Policy" section of the Play Console

3. The policy covers all required elements for Play Store compliance:
   - Data collection practices (none by developer)
   - Permission usage explanations
   - Third-party services
   - User rights
   - Contact information
   - GDPR/CCPA compliance

## Custom Domain (Optional)

If you want to use a custom domain:

1. Add a file named `CNAME` to the `/docs` directory
2. Put your custom domain in the file (e.g., `privacy.defencebay.com`)
3. Configure your DNS provider to point to GitHub Pages:
   - Add a CNAME record pointing to `<username>.github.io`
   - Or add A records pointing to GitHub's IPs

See: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Updating the Privacy Policy

To update the privacy policy:

1. Edit `privacy-policy.html` (this is the main file shown to users)
2. Update `privacy-policy.md` to match (for reference/documentation)
3. Update the "Last Updated" date at the top
4. Commit and push the changes
5. GitHub Pages will automatically redeploy (1-2 minutes)

## Troubleshooting

### Privacy policy not showing up?
- Check that GitHub Pages is enabled in Settings > Pages
- Ensure you selected `/docs` as the folder
- Wait a few minutes for deployment
- Check the Actions tab for build errors

### 404 Error?
- Verify the URL includes your username and repository name
- Check that files are in the `/docs` directory
- Ensure the branch you selected in Pages settings contains the `/docs` folder

### Need to test locally?
You can test the privacy policy locally by:
```bash
cd docs
python3 -m http.server 8000
```
Then visit: http://localhost:8000/privacy-policy.html

## Support

For questions about the privacy policy or setup:
- Create an issue in this repository
- Contact DefenceBay at biuro@mzeds.pl

## License

The privacy policy is part of the TROP project and follows the same licensing as ATAK-CIV (GPLv3).
