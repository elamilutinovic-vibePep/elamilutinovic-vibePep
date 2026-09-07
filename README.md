# Hi, I'm Ela 👋

I focus on **Supabase backend architecture, authorization security, and maintainable PostgreSQL design**.

I review and diagnose authentication, Row Level Security, RPC, Edge Function, Storage, and multi-tenant data-access problems. My approach is to identify the actual execution context, reproduce the failure, and verify the fix across ownership boundaries.

## Core areas

- Supabase Auth and authorization context
- Row Level Security design and debugging
- Database functions and RPC security
- Edge Function → RPC → PostgreSQL boundaries
- Multi-tenant ownership and data integrity
- Controlled SQL migrations and reproducible verification

## Selected public work

### [Supabase Security Labs](https://github.com/elamilutinovic-vibePep/supabase-security-labs)

Reproducible case-study labs covering broken and corrected RLS isolation, user JWT versus `service_role` execution context, Edge and database authorization boundaries, private Storage, and protected membership sources.

### [Supabase Patterns](https://github.com/elamilutinovic-vibePep/supabase-patterns)

Tested patterns for owner-only RLS, authenticated RPC operations, and Edge → RPC → RLS flows, with two-user isolation tests, security-review guidance, and explicit scope limitations.

## Private backend case study

**Little Biker** uses separate parent and child authorization contexts, avatar-and-PIN child access, short-lived sessions, rate limiting, RLS, RPCs, Edge Functions, and migration-based database development. The source code is private; related security patterns are demonstrated independently in the public repositories above.

## Working approach

- Understand the ownership model before writing policies.
- Treat the database as the final authorization boundary.
- Test with at least two identities across an ownership or tenant boundary.
- Describe only behavior that has actually been demonstrated.

## Contact

Portfolio and contact: [vibepep.com](https://vibepep.com)
