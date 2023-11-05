## What is Seed Job?

- A seed job is a normal Jenkins job that creates and updates other jobs.
- The seed job is the first job that you run to set up your Jenkins environment.
- The seed job is a Jenkins job which runs a DSL scripts, and then generates a new job.
- The seed job is the first job that you run to set up your Jenkins environment.
- The seed job is a Jenkins job which runs a DSL scripts, and then generates a new job.

### Configuring Seed Job:

1. Click on "New Item."
2. Enter the name of the job.
3. Select "Freestyle project."
4. Click on "OK."
5. Click on Configure.
6. Select Source Code Management as "Git."

7. Click on Build Step and select "Process Job DSLs."

