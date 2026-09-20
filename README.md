# Grant Obligation Tracker

Private development repository for **GrantPilot** (working codename), a simple, privacy-first post-award grant obligation tracker for small nonprofits.

## MVP capabilities
- Create and view grant awards
- Create award-level obligations with internal and funder deadlines
- Assign owners and track evidence requirements
- Dashboard for open, due-soon, and overdue obligations
- IndexedDB local persistence; no account or application server required
- JSON backup export
- Responsive interface

## Run locally

```bash
npm install
npm run dev
```

## Build and test

```bash
npm run build
npm test
```

## Privacy
MVP grant data is stored locally in the browser via IndexedDB and is not transmitted to an application server.

## Status
Private development prototype. **GrantPilot is a working codename, not a cleared public brand.**
