# dotnet-core-hello-world
This is a simple dotnet application hosting helloworld page using Cloud Foundry.

Deploying to Cloud Foundry
After installing in the 'cf' command-line interface for Cloud Foundry, targeting a Cloud Foundry instance, and logging in, the application can be pushed using these commands:
$ git clone <repo_link>
$ cd dotnet-core-hello-world
$ cf push
...
Push successful! App is now available at http://<route_name>.cfapps.io
The provided manifest.yml file will be used to provide the application parameters to Cloud Foundry. A unique URL will be assigned to the application, which is shown at the end of the output from 'cf push'. The manifest.yml file specifies a RabbitMQ services that is available on the run.pivotal.io Cloud Foundry services marketplace. You may need to change the details of the RabbitMQ service to push to a different Cloud Foundry instance.

