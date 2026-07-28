# Security Notes

This repository is a portfolio edition of a BSc final-year academic project and should **not** be deployed as a production election platform without further security work.

## Known Legacy Concerns

The original implementation contains patterns typical of an undergraduate/legacy PHP project, including:

- MD5/plain-text style password handling in parts of the authentication flow;
- SQL statements constructed from request values in some files;
- legacy `mysql_*` usage alongside `mysqli`;
- development-oriented database configuration;
- limited CSRF/input-validation protections.

## Recommended Production Improvements

1. Replace legacy password handling with `password_hash()` and `password_verify()`.
2. Replace interpolated SQL with prepared statements throughout.
3. Centralise database configuration and load credentials from environment variables.
4. Add CSRF protection to state-changing forms.
5. Validate and encode all user-controlled input/output.
6. Apply least-privilege database permissions.
7. Add server-side enforcement for election eligibility and one-vote-per-position constraints.
8. Add automated tests, audit logging and secure session/cookie configuration.

The repository is intended to demonstrate the system design and software-development work completed for the academic project, while documenting the engineering changes required for a modern production implementation.
