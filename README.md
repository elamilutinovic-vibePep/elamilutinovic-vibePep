# Hi, I'm Ela 👋

I focus on **Supabase backend architecture, authorization security, and maintainable PostgreSQL design**.

I review and diagnose authentication, Row Level Security, RPC, Edge Function, Storage, and multi-tenant data-access problems. My approach is to identify the actual execution context, reproduce the failure, and verify the fix across ownership boundaries.

## Focus

- Supabase Auth and authorization context
- Row Level Security design and debugging
- Database functions and RPC security
- Edge Function → RPC → PostgreSQL boundaries
- Multi-tenant ownership and data integrity
- Controlled SQL migrations and reproducible verification

## Selected public work

### [Supabase Security Labs](https://github.com/elamilutinovic-vibePep/supabase-security-labs)

Reproducible case-study labs for investigating common Supabase authorization failures.

The labs cover:

- broken and corrected RLS isolation;
- user JWT versus `service_role` execution context;
- Edge Function and database authorization boundaries;
- private Storage and tenant-path isolation;
- protected membership sources;
- repeatable setup and verification workflows.

### [Supabase Patterns](https://github.com/elamilutinovic-vibePep/supabase-patterns)

Focused backend patterns for owner-only RLS, authenticated RPC operations, and Edge → RPC → RLS request flows.

The repository includes:

- SQL schemas, policies, functions, and grants;
- automated two-user ownership-isolation tests;
- direct RPC boundary and validation tests;
- a structured Supabase security-review checklist;
- a fast initial backend security-triage procedure;
- explicit scope and limitation notes for every example.

## Private project work

### Little Biker

A private Supabase backend project designed around parent and child access with separate authorization contexts.

Implemented areas include:

- parent authentication and child avatar + PIN access;
- short-lived child sessions and session revocation;
- rate-limited PIN verification;
- RLS, RPC, and Edge Function responsibility boundaries;
- parent-owned family data and child-safe lesson access;
- migration-based database development.

The source code is private. Related authorization patterns are demonstrated independently in my public repositories.

## Working principles

- Understand the ownership model before writing policies.
- Treat the database as the final authorization boundary.
- Use privileged access only through explicit, reviewable authorization.
- Test with at least two identities across an ownership or tenant boundary.
- Keep migrations, documentation, and verification aligned with the implementation.
- Describe only behavior that has actually been demonstrated.

## Contact

Portfolio and contact: [vibepep.com](https://vibepep.com)
