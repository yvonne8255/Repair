# Mechanic 维修工作板

Vehicle repair job board (中文 / EN), styled to the Pollisum style guide. Static page (`index.html`) + Supabase backend.

- Backend: Supabase project `mechanic-board` (tables `profiles`, `cases` with row-level security; edge function `account` for register / update user / delete user).
- Login is phone number + password (stored as a synthetic email `p<digits>@mechanic.invalid`). The first person to register becomes Admin; everyone else waits for Admin approval.
- Roles: Admin, Mechanic, Operation. Permissions are enforced by row-level security and the edge function.
- The 512-vehicle list from Book1.xlsx is embedded in `index.html`.
