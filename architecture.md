# Architecture Overview

The Fintech Data Marketplace uses a three-tier architecture:

1. **Frontend** – React.js SPA for browsing, searching, and requesting datasets.
2. **Backend API** – Node.js/Express (or Python/FastAPI) for handling requests, metadata retrieval, and authentication.
3. **Database** – Stores dataset metadata, user permissions, and request logs.

## Security Model
- Only authenticated users can request datasets
- All requests logged for auditing
- No direct download links; access is via approved workflows

## Data Sample Policy
- Each dataset may expose a small anonymized preview
- Owners approve requests before granting access
