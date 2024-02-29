Flyway Autopilot allows you to trial an end-to-end database development and automated deployment process with very little setup.  With Flyway AutoPilot for PostgreSQL, you get: 

## What's Included
1. Two SQL scripts to create the required sample databases (`1-create_autopilot_databases.sql`) and populate each with the initial schema (`2-create_initial_database_schema.sql`)
2. A pre-configured Flyway project to get started quickly
3. Integration with version control to track your changes and collaborate with a team
4. Example migration scripts that are already deployed to the sample databases and the ability to generate new migration scripts (both versioned and undo scripts)
5. A GitHub Actions pipeline to facilitate Continuous Integration and Continuous Deployments (CI/CD) across the sample databases
6. Reports to provide more visibility and safety checks integrated into the pipeline

## Requirements
1. A running PostgreSQL instance, preferably local to your machine.
   - [Docker](https://hub.docker.com/_/postgres) is often the easiest way to do this if PostgreSQL is not already available.
2. A compatible IDE like [DBeaver](https://dbeaver.io/download/) or the `psql` command line tool if you're comfortable with that.
3. A GitHub account
4. `git` tooling installed locally and accessible in your path.
5. Flyway Enterprise installed and activated locally. This can be a trial or fully licensed version.

## Getting your environment setup
To follow along with the Quickstart guide linked below, you need to run the two SQL scripts included in the repository.

1. Connect to any database with a user that has the `CREATEDB` privilege (the `postgres` user in the Docker container does).
2. Execute the `1-create_autopilot_databases.sql` script to create all of the databases used in this Quickstart sample. All databases start with the name `widget`.
3. Now one by one, connect to each of the `widget` databases and execute the `2-create_initial_database_schema.sql` scripts. This will create a few tables, a view, and a function.

You're now ready to follow the rest of the Quickstart, which includes setting up a local GitHub Actions runner to see the CI/CD pipeline work with your local databases.

**Check out the [documentation to get started](https://documentation.red-gate.com/fd/quickstart-flyway-autopilot-215154689.html)**.
