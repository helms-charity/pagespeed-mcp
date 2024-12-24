# MCP PageSpeed Server

A local server implementation that provides PageSpeed Insights API functionality for testing web performance metrics.

## Features

- Run PageSpeed tests on any URL
- Get detailed performance metrics including:
  - Loading performance (FCP, LCP, TTI)
  - Layout stability (CLS)
  - Interactivity (TBT, TTI)
- Security and best practices audits
- Accessibility testing
- SEO analysis

## Installation

1. Download the server files
2. Ensure you have Node.js installed
3. Run `npm install` to install dependencies

## Usage

1. Start the server:
```bash
npm start
```

2. Make API calls to `http://localhost:3000/pagespeed` with the following parameters:
- `url`: The URL to test (required)
- `strategy`: Either 'mobile' or 'desktop' (default: mobile)
- `category`: Array of categories to test ['performance', 'accessibility', 'best-practices', 'seo']

Example API call:
```javascript
fetch('http://localhost:3000/pagespeed?url=https://example.com')
```

## API Response

The server returns a detailed JSON response containing:
- Performance metrics
- Loading statistics
- Resource optimization suggestions
- Best practices audit results
- Accessibility findings
- SEO recommendations

## Requirements

- Node.js v14 or higher
- Modern web browser for testing
- Internet connection for testing external URLs

## License

MIT License

## Contributing

Contributions are welcome! Send over your PR.

## Support

For issues and feature requests, please use the GitHub issue tracker.