# Installing via Docker

1. Install docker according to [instructions](https://docs.docker.com/engine/installation/).
2. Pull orienteer image by the following command: `docker pull orienteer/orienteer`. For more details check [docker hub repository](https://hub.docker.com/r/orienteer/orienteer/).
3. Run new container by command `docker run -p 8080:8080 orienteer/orienteer`. Adjust this command if needed.
   1. You can supply required orienteer properties values with the aid of environments properties. Please use correct naming convention: uppercase and underscore instead of dots. For example to specify `orienteer.admin.password` you should write `-e ORIENTEER_ADMIN_PASSWORD=password`

## Using Docker Cloud

[Docker Cloud](https://cloud.docker.com) is great thing for deployment \(and even automatic redeployment\) of a solution on your own promises.

1. Register on [Docker Cloud](https://cloud.docker.com)
2. Add node: either use AWS, DigitalOcean services or "Bring your node"
3. Create new service from `orienteer/orienteer:latest` public image. It's recommended to set "autoredeploy" and setup volume for `/orienteer/Orienteer`
4. Create new container for this service. Map container port to required external port.
5. After container deployment completion: just go to container URL.



