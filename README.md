# scalar-static

A static API documentation site powered by [Scalar](https://github.com/scalar/scalar), featuring an interactive OpenAPI specification viewer.

## 📁 Files

- **index.html** - Main HTML page that loads the Scalar API reference viewer
- **openapi-v1.yaml** - Sample OpenAPI 3.1.0 specification with example API endpoints

## 🚀 Usage

### Option 1: Local Development Server

Serve the files using a local web server to avoid CORS issues:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve

# Using PHP
php -S localhost:8000
```

Then open http://localhost:8000 in your browser.

### Option 2: Direct File Access

Simply open `index.html` in your web browser. Note that some browsers may block the CDN resources when opening files directly (file:// protocol).

### Option 3: Deploy to GitHub Pages

1. Go to your repository settings
2. Navigate to Pages section
3. Select the branch and root directory
4. Your documentation will be available at `https://<username>.github.io/<repository>/`

## 📝 Sample API Overview

The included OpenAPI specification demonstrates:

- **Users API** - Create, read, update, and delete user accounts
- **Posts API** - Manage blog posts with full CRUD operations
- **Authentication** - API key-based authentication
- **Pagination** - Paginated list endpoints
- **Error Handling** - Comprehensive error responses

## 🔧 Customization

### Update the OpenAPI Specification

Edit `openapi-v1.yaml` to define your own API endpoints, schemas, and documentation.

### Customize Scalar Appearance

You can customize Scalar's appearance by modifying the script tag in `index.html`:

```html
<script
    id="api-reference"
    data-url="./openapi-v1.yaml"
    data-theme="purple"></script>
```

See [Scalar documentation](https://github.com/scalar/scalar) for more configuration options.

## 📚 Resources

- [Scalar GitHub Repository](https://github.com/scalar/scalar)
- [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Scalar Configuration Options](https://github.com/scalar/scalar#configuration)

## 📄 License

This project is open source and available under the MIT License.