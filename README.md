# Singh Eye Hospital Screenshots Repository

This repository hosts UI screenshots used in pull request reviews for the [Singh Eye Hospital React Frontend](https://github.com/akshatsinghkaushik/singh-eye-hospital-react).

## Purpose

This public repository serves as a CDN for screenshot assets, keeping the main application repository clean while providing fast, reliable access to UI proof images used in the development workflow.

## Structure

```
screenshots/
├── current/           # Latest screenshots from main branch
└── archive/          # Historical screenshots organized by timestamp
    ├── YYYYMMDD_HHMMSS/
    │   ├── homepage-desktop.png
    │   ├── homepage-mobile.png
    │   ├── homepage-tablet.png
    │   ├── homepage-button-hover.png
    │   ├── homepage-full.png
    │   └── homepage-viewport.png
    └── ...
```

## Automated Management

This repository is automatically managed by CI/CD scripts from the main application repository. Screenshots are:

- **Generated**: Using Playwright automation during PR creation
- **Uploaded**: Automatically via GitHub Actions and CLI scripts
- **Organized**: By timestamp and branch information
- **Cleaned**: Old screenshots are periodically archived or removed

## URL Pattern

Screenshots are accessible via GitHub's raw content URLs:

```
https://raw.githubusercontent.com/akshatsinghkaushik/singh-eye-hospital-screenshots/main/screenshots/{path}/{filename}.png
```

## Integration

These screenshots are embedded in PR descriptions using HTML img tags with appropriate sizing for optimal review experience:

```html
<img src="https://raw.githubusercontent.com/akshatsinghkaushik/singh-eye-hospital-screenshots/main/screenshots/archive/YYYYMMDD_HHMMSS/homepage-desktop.png" alt="Desktop View" width="600" />
```

## Maintenance

- **Retention**: Screenshots are kept for historical reference
- **Organization**: Organized by generation timestamp
- **Access**: Public read access for PR review integration
- **Management**: Automated via main repository workflows

---

**Related Repository**: [Singh Eye Hospital React Frontend](https://github.com/akshatsinghkaushik/singh-eye-hospital-react)  
**Automation**: This repository is managed by automated scripts and workflows
