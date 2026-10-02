# Notes v5 — Blue Productivity Workspace

A standalone Next.js notes app with a structured list and desktop split-view editor.

## Run it

```bash
npm install
npm run dev
```

Open `http://localhost:3000`. For verification, run:

```bash
npm run typecheck
npm run build
```

## Requirement mapping

- `app/page.tsx`: `useState` state, `useEffect` load/save/duplicate checks, validation, feedback, confirmation, and localStorage error handling.
- `components/NoteItem.tsx`: separate note row component with edit and delete actions.
- Add, view, edit, and delete are all functional. Titles are normalized with `trim()`, lowercase conversion, and repeated-whitespace collapsing; editing excludes the current note ID.
- Storage key: `notefolio-notes-workspace-v5`.
- `app/globals.css`: productivity split view plus desktop, tablet, and 360px-friendly responsive rules, focus states, readable contrast, and touch-sized controls.
- No backend, login, or remote data is used.
