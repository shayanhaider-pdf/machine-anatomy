# Publish Machine Anatomy with GitHub Pages

The source code is already public in this repository. The workflow at `.github/workflows/deploy-pages.yml` uploads the full static HTML gallery, models and documentation.

## Required one-time owner action

GitHub rejected automatic Pages creation by the Actions integration. As the repository owner:

1. Open https://github.com/shayanhaider-pdf/machine-anatomy/settings/pages
2. Under **Build and deployment**, choose **GitHub Actions** as the source. Save or enable Pages if GitHub requests it.
3. Open https://github.com/shayanhaider-pdf/machine-anatomy/actions/workflows/deploy-pages.yml
4. Select **Run workflow**, choose `main` and run it.
5. Once the workflow reports success, the canonical gallery URL is expected to be https://shayanhaider-pdf.github.io/machine-anatomy/ and the combined simulator at https://shayanhaider-pdf.github.io/machine-anatomy/pharma/

The original GitHub Actions run (November 14, 2026) reached `Configure GitHub Pages` but GitHub returned: `Resource not accessible by integration` when attempting to create the Pages site. The workflow is present and can be re-run after the one-time owner setting.

## Other ways to use it

You can inspect all repository files in GitHub without Pages. For HTML rendering, a third-party static GitHub preview URL is linked from the README, but those preview services are not controlled by this repository and may have their own caching or access rules.

The HTML files also run without external dependencies if saved and opened in a normal browser.
