# API Scenarios

## Core Endpoints
- POST /api/transactions/start
- POST /api/transactions/{id}/items
- POST /api/transactions/{id}/submit
- GET /api/transactions/{barcode}
- POST /api/transactions/{id}/complete
- POST /api/transactions/{id}/reprint

## Validation Points
- transaction id created once and reused
- duplicate item scans handled correctly
- submit fails gracefully when backend unavailable
- barcode lookup returns exact basket
- completed basket cannot be resubmitted
- reprint allowed only for most recent eligible basket
