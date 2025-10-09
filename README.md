# MSP REST API Documentation

This directory contains the Swagger UI documentation for the MSP (Member Service Provider) REST API.

## Files

- `index.html` - Main Swagger UI interface with custom theming
- `custom-theme.css` - Custom CSS theme for professional appearance
- `MSP_REST_API_Swagger.yaml` - OpenAPI 3.0.3 specification (auto-updated)

## Features

- **Automatic Updates**: The YAML file is automatically updated when changes are pushed to the main branch
- **Custom Theme**: Professional styling with Exium branding colors
- **GitHub Pages**: Automatically deployed to GitHub Pages
- **Responsive Design**: Works on desktop and mobile devices
- **Interactive Testing**: Try out API endpoints directly in the browser

## Deployment

The documentation is automatically deployed to GitHub Pages when:

1. Changes are pushed to the `main` or `master` branch
2. The `MSP_REST_API_Swagger.yaml` file is updated
3. Any files in the `docs/` directory are modified

## Customization

### Theme Colors

The theme uses CSS custom properties that can be easily modified:

```css
:root {
    --primary-color: #2c3e50;      /* Dark blue-gray */
    --secondary-color: #3498db;    /* Blue */
    --accent-color: #e74c3c;       /* Red */
    --success-color: #27ae60;      /* Green */
    --warning-color: #f39c12;      /* Orange */
}
```

### Adding New Features

To add new features to the Swagger UI:

1. Modify the `index.html` file
2. Update the SwaggerUIBundle configuration
3. Add any additional CSS to `custom-theme.css`

## Local Development

To test the documentation locally:

1. Serve the `docs/` directory using a local web server
2. Example with Python: `python -m http.server 8000` in the docs directory
3. Open `http://localhost:8000` in your browser

## API Information

- **Title**: MSP (Member Service Provider) REST API
- **Version**: 1.0.0
- **Contact**: support@exium.net
- **License**: Proprietary

## Endpoints

The API provides comprehensive management for:

- **MSP Management**: Create, read, update, and delete MSPs
- **MSP User Management**: Manage users within MSPs
- **Authentication**: Session-based authentication with X-Auth-Token header

## Security

All endpoints require session-based authentication using the `X-Auth-Token` header.
