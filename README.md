# Mechanic 维修工作板

Vehicle repair job board (中文 / EN), styled to the Pollisum style guide.

- `index.html`: the whole app in one file, with the 512-vehicle list from Book1.xlsx embedded.
- Needs the claude.ai Artifact `db` runtime (shared `users` and `cases` collections) to store data. Opened outside that runtime it shows "cannot reach the database".
- Roles: Admin, Mechanic, Operation. The first person to register becomes Admin; everyone else needs approval.
- Permissions are enforced in the page, not in the database.
