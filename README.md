# TP DevOps Correction Docker

Correction de la partie Docker du module DevOps. Amusez-vous bien avec GitHub Actions !

What are testcontainers?  
Testcontainers is a Java library which allow Docker containers in our automate test. It allows you to test services like a Postgres DB in our example2-2  

For what purpose do we need to use secured variables ?  
Secured Variables are used to protect informations like credentials in our workflows2-3  

Why did we put needs: build-and-test-backend on this job?  
Maybe try without this and you will see ! We put needs for this jon because there is a dependance of the build and push with the test backend. The build and push will publish images only if the test wackend is completed. It allows to publish images only if the quality code is sufficient and the compilation passed good**CD is the next logigal step of CI**2-4  

For what purpose do we need to push docker images ?  
Pushing a Docker image makes the application easily deployable and shareable across environments without rebuilding.It enables versioning, supports Continuous Delivery, and is essential for deployment automation.
