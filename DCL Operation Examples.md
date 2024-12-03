# Examples of DCL Operations

# 1. GRANT

Q: Display the query to grant the SELECT privilege on the employees table to a user named john_doe.

GRANT SELECT ON employees TO john_doe;

# 2. GRANT with MULTIPLE PRIVILEGES

Q: Display the query to grant SELECT, INSERT, and UPDATE privileges on the employees table to a user named jane_doe.

GRANT SELECT, INSERT, UPDATE ON employees TO jane_doe;

# 3. GRANT ALL PRIVILEGES

Q: Display the query to grant all privileges on the employees table to a user named admin_user.

GRANT ALL PRIVILEGES ON employees TO admin_user;

# 4. REVOKE

Q: Display the query to revoke the SELECT privilege on the employees table from the user john_doe.

REVOKE SELECT ON employees FROM john_doe;

# 5. REVOKE ALL PRIVILEGES

Q: Display the query to revoke all privileges on the employees table from the user jane_doe.

REVOKE ALL PRIVILEGES ON employees FROM jane_doe;

# 6. GRANT with OPTION

Q: Display the query to grant the SELECT privilege on the employees table to john_doe, allowing john_doe to grant SELECT privileges to others.

GRANT SELECT ON employees TO john_doe WITH GRANT OPTION;

# 7. GRANT USAGE on SCHEMA

Q: Display the query to grant USAGE privilege on a schema hr_schema to a user john_doe.

GRANT USAGE ON SCHEMA hr_schema TO john_doe;

# 8. REVOKE USAGE on SCHEMA

Q: Display the query to revoke the USAGE privilege on the schema hr_schema from the user john_doe.

REVOKE USAGE ON SCHEMA hr_schema FROM john_doe;
