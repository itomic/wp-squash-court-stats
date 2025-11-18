# Squash Court Stats WordPress Plugin

WordPress plugin for embedding dashboards and reports from [stats.squashplayers.app](https://stats.squashplayers.app) into WordPress pages using shortcodes.

## Installation

1. Download the latest release from [GitHub Releases](https://github.com/itomic/wp-squash-court-stats/releases)
2. Upload `squash-court-stats.zip` to WordPress (Plugins → Add New → Upload Plugin)
3. Activate the plugin

## Usage

### Dashboards

```
[squash_court_stats dashboard="world"]
[squash_court_stats dashboard="trivia"]
```

### Reports

```
[squash_court_stats report="graveyard"]
[squash_court_stats report="nearest-courts"]
```

### Charts

```
[squash_court_stats charts="world-map,top-countries"]
```

See [docs/wordpress-plugin/SHORTCODE-USAGE-GUIDE.md](docs/wordpress-plugin/SHORTCODE-USAGE-GUIDE.md) for complete documentation.

## Development

### Packaging

```powershell
.\package-plugin.ps1
```

Or for WordPress.org submission:

```powershell
.\package-plugin-wporg.ps1
```

### Testing

The plugin can be tested locally by:
1. Installing in a local WordPress instance
2. Using the shortcodes on test pages
3. Checking browser console for any errors

## Repository Structure

```
wp-squash-court-stats/
├── squash-court-stats.php      # Main plugin file
├── readme.txt                   # WordPress.org readme
├── includes/                   # Plugin classes
│   └── class-plugin-updater.php
├── docs/                       # Documentation
│   └── wordpress-plugin/
├── .github/                    # GitHub Actions workflows
│   └── workflows/
│       └── release.yml
└── package-plugin.ps1          # Packaging script
```

## License

GPL v2 or later

## Links

- **Plugin Source**: This repository
- **Dashboard Source**: [squash-court-stats](https://github.com/itomic/squash-court-stats) (Laravel application)
- **Live Dashboard**: https://stats.squashplayers.app

