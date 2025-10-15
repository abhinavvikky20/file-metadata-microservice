# File Metadata Microservice

## Overview
This is a File Metadata Microservice built with Node.js and Express. It's a freeCodeCamp API project that allows users to upload files and receive metadata information about them (filename, file type, and file size).

## Project Status
- **Last Updated**: October 15, 2025
- **Status**: Fully configured and running in Replit environment

## Recent Changes
- Configured to run on port 5000 with 0.0.0.0 binding for Replit environment
- Added multer middleware for file upload handling
- Implemented `/api/fileanalyse` endpoint to process file uploads
- Added uploads/ directory to .gitignore
- Configured deployment for autoscale

## Project Architecture

### Tech Stack
- **Runtime**: Node.js
- **Framework**: Express.js
- **Dependencies**:
  - cors: Cross-origin resource sharing
  - dotenv: Environment variable management
  - multer: File upload middleware

### File Structure
```
├── index.js           # Main server file
├── package.json       # Node.js dependencies
├── views/
│   └── index.html     # Frontend HTML
├── public/
│   └── style.css      # Styling
└── uploads/           # Temporary file upload storage (gitignored)
```

### API Endpoints
- `GET /` - Serves the main HTML interface
- `POST /api/fileanalyse` - Accepts file uploads and returns metadata:
  - name: original filename
  - type: MIME type
  - size: file size in bytes

## Configuration
- Server listens on port 5000 (configured via PORT environment variable)
- Binds to 0.0.0.0 for Replit proxy compatibility
- File uploads stored temporarily in uploads/ directory
- Deployment configured for autoscale (stateless)

## User Preferences
None documented yet.
