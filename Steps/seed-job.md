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

![dsl-6](https://github.com/mathesh-me/dsl-approach-jenkins-project/assets/144098846/2f0465db-7783-44b6-ba89-27b8c39c3cfb)

7. Click on Build Step and select "Process Job DSLs."

![dsl-5](https://github.com/mathesh-me/dsl-approach-jenkins-project/assets/144098846/61f966db-ae1c-444c-857e-561e156f8152)

![dsl-7](https://github.com/mathesh-me/dsl-approach-jenkins-project/assets/144098846/1bedfcc2-19b2-47ad-a2eb-52e4b2bf355a)
