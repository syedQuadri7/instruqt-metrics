# instruqt-api-client

Requirements: Python version 3.11.3 (global), Doormat access, Code editor (VScode)

1. Request short-term project for Doormat
    1. Enable APIs
    2. Select ‘APIs and Services’
    3. Enable Sheets API
    4. Enable Drive API
2. Generate Credentials
    5. Select ‘APIs and Services’
    6. Select ‘Credentials’
    7. Select “+ Create Credentials”
    8. Select “Service Account” and fill in details
    9. Click on Service Account name (created in Step 4)
    10. Click the ‘Keys’ tab
    11. Click ‘Add Key’
    12. Select ‘JSON’
    13. Click ‘Create’
    14. Save Credentials file locally
3. This currently maps to Env var:
    15. “GOOGLE_SPREADSHEET_CREDENTIALS”
    16. Rename to ‘creds.json’
    17. Move it into current directory (where code lives)
4. Open file created in Step 2 copy the ‘client_email’
5. In Google Sheets
    18. Select File -> Share -> Share with Others
    19. Add client_email with ‘Editor’ permissions
6. Make sure you have an API key, this can be generated by an owner of the instruqt org. You may also use an existing key. Note: There can only be one at a time so make sure this key isn't being used anywhere else
7. In script.sh
    20. Replace the INSTRUQT_TOKEN with the most recent API key
8. In the terminal run script.sh by running the following
    21. ./script.sh
    22. The google sheet should be updated. Process takes about 5-10 min