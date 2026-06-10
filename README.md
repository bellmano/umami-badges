# :ramen: Umami Badges 

[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=coverage&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=security_rating&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=sqale_rating&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=reliability_rating&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=bugs&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=vulnerabilities&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=bellmano_umami-badges&metric=code_smells&token=6e9bb50bb14b2d851f65c161bef4a5e41dc5050c)](https://sonarcloud.io/summary/overall?id=bellmano_umami-badges)

Generate dynamic badges for your Umami website analytics! Show off your website traffic, page views, and visitor stats directly in your README files or on your website.

## :rocket: Quick Start

### 1. Get Your Website ID and API Key

You'll need:
- Your Website ID (found in your website settings)
- An API key (Account Settings → API keys)

**:warning: Security Notice:** Your API key will be visible in the badge URL. This means anyone can view your website analytics data (views, visitors, etc.) but cannot modify settings or access other websites. Only use badges for public websites where you're comfortable sharing traffic statistics. You can rotate your API key anytime in Umami settings.

### 2. Generate Your Badge

**Option A: Use the Web Interface**

Visit: **[umami-badges.vercel.app](https://umami-badges.vercel.app/)**

**Option B: Build the URL yourself**

Default (Umami Cloud):
```
https://umami-badges.vercel.app/api/{metric}?website={WEBSITE_ID}&token={API_TOKEN}&range=all&style=for-the-badge&cache=0
```

Self‑hosted or custom domain (add `umamiUrl`):
```
https://umami-badges.vercel.app/api/{metric}?website={WEBSITE_ID}&token={API_TOKEN}&range=all&style=for-the-badge&cache=0&umamiUrl={CUSTOM_UMAMI_API_URL}
```

### 3. Add to Your README

```markdown
![Website Analytics](https://umami-badges.vercel.app/api/views?website=your-website-id&token=your-api-token&range=all&style=for-the-badge&cache=0)
```

## :bar_chart: Available Metrics

| Metric | Description | Example |
|--------|-------------|---------|
| `views` | Total page views | ![Views](https://img.shields.io/badge/Views-12.5K-brightgreen?style=for-the-badge) |
| `visitors` | Unique visitors | ![Visitors](https://img.shields.io/badge/Visitors-3.2K-green?style=for-the-badge) |
| `visits` | Total visits | ![Visits](https://img.shields.io/badge/Visits-8.9K-blue?style=for-the-badge) |
| `bounce-rate` | Bounce rate percentage | ![Bounce Rate](https://img.shields.io/badge/Bounce%20Rate-45.2%25-orange?style=for-the-badge) |
| `avg-session` | Average session duration | ![Avg Session](https://img.shields.io/badge/Avg%20Session-1m_36s-purple?style=for-the-badge) |
| `live` | Live visitors (last 30 minutes) | ![Live](https://img.shields.io/badge/Live%20Visitors-42-red?style=for-the-badge) |

## :art: Customization Options

| Parameter | Description | Values |
|-----------|-------------|--------|
| `range` | Time range for stats | `7d`, `30d`, `90d`, `all` (default: `all`) |
| `style` | Badge style | `flat`, `flat-square`, `for-the-badge`, `plastic`, `social` |
| `color` | Badge color | `brightgreen`, `green`, `blue`, `red`, `orange`, `yellow`, `purple`, or hex codes |
| `label` | Custom label text | Any text (URL encoded) |

## :test_tube: Running Tests

To run the tests and view coverage:

1. Install the required dev dependency:
	```powershell
	npm install
	```
2. Run the test coverage script:
	```powershell
	npm run test:coverage
	```

This will execute the tests and generate a coverage report.

## :handshake: Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## :mega: Issues or Suggestions
Any issues or suggestions, please [create an issue on Github](https://github.com/bellmano/umami-badges/issues).

## :coffee: Buy me a coffee
Donations are welcome to appreciate my work and to keep this project alive, but isn't required at all.

<a href="https://ko-fi.com/bellmano"><img src="img/bellmano-kofi.jpg" width="50%"></a>
