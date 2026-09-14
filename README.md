# Your accessibility audit

This repository is ready to run the free [CarlasHub WCAG Accessibility Audit](https://github.com/CarlasHub/accessibility-audit-plugin) in GitHub Actions. The audit and its report run in **your repository**, under **your GitHub account**—not on CarlasHub infrastructure.

## Run your first audit

1. Open the [Accessibility audit workflow](../../actions/workflows/accessibility-audit.yml).
2. Select **Run workflow**.
3. Paste one public `https://` page per line in **Public HTTPS pages to audit**. You can include up to 20 pages.
4. Select the green **Run workflow** button.
5. Open the new run and wait for the **Audit website** job to finish.
6. Use **Download the complete report** in the run summary. The ZIP contains an accessible HTML report, Excel workbook, JSON evidence, screenshots, and supporting files.

Example page list:

```text
https://example.com/
https://example.com/contact
https://example.com/help
```

## What the audit covers

The Action combines automated WCAG 2.2 checks with keyboard, focus, responsive reflow, and guided manual-review evidence. It tests only the exact pages you enter; it does not crawl an entire website.

Automated results cannot certify WCAG conformance. Screen-reader experience, content meaning, usability, and exceptions still require human review.

## Use it safely

Only audit websites you own or are authorised to test. Avoid URLs containing passwords, private tokens, or other credentials. GitHub controls the Actions usage, artifacts, retention, and permissions in this repository.

For advanced inputs, staging sites, quality gates, pull-request comments, and local integrations, see the [complete documentation](https://github.com/CarlasHub/accessibility-audit-plugin#readme).

---

Maintained by [CarlasHub](https://carlashub.com/) and provided under the [MIT License](https://github.com/CarlasHub/accessibility-audit-plugin/blob/main/LICENSE).
