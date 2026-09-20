# Privacy Model

## Alpha implementation review

The current Alpha is local-first.

- No login or user account is required.
- No application-server database is used.
- Grant and obligation records are stored in the user's browser with IndexedDB (database name: `GrantPilot`).
- The application code does not intentionally send grant or obligation records to an application server, analytics service, or paid API.
- JSON backup and CSV export are generated in the browser and downloaded by the user.
- JSON/CSV restore reads the file selected by the user in the browser.
- No grant documents are uploaded or stored by the application.
- No analytics or tracking SDK is included in the current source.

## Important limitations

Browser-local storage belongs to the browser/device profile. Clearing site data, changing browsers/devices, or losing the device can remove locally stored records. Users should export backups regularly.

Hosting the static application will necessarily involve normal web-host request metadata handled by the hosting provider, but the current application does not intentionally submit grant-record contents to that provider.

This review describes the private Alpha implementation as of Phase 6. It must be reviewed again before a public release or whenever hosting, analytics, accounts, cloud synchronization, APIs, or document storage are introduced.
