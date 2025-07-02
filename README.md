# ZIP Radius Mapper

An interactive web application that allows users to upload location data, map it, and find locations within a specified radius of any ZIP code.

## Features

- Upload Excel (.xlsx/.xls) or CSV files with location data
- Automatically map locations with latitude/longitude coordinates
- Search for locations within a specified radius of any ZIP code
- View a catalog of all mapped locations

## Development Setup

### Prerequisites

- Node.js and npm installed

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd zip-radius-mapper
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

### Development Server

Run the development server:

```bash
npm start
```

This will open the application in your default browser at `http://localhost:3000`.

### Building for Production

Create a production build:

```bash
npm run build
```

This will copy all files from the `src` directory to the `dist` directory. The `dist` directory is used for production-ready files and is not tracked in version control.

**Note:** The `dist` folder is automatically generated when running the build command and can be safely deleted when not needed. It will be recreated whenever you run `npm run build`.

## Deployment

The application can be deployed to any static hosting service like AWS S3, Netlify, or GitHub Pages.

## API Key

This application uses the Geoapify API for geocoding ZIP codes. The API key is included in the source code for demonstration purposes. For production use, consider:

1. Moving the API key to environment variables
2. Setting up domain restrictions for the API key
3. Using a server-side proxy to make API calls
