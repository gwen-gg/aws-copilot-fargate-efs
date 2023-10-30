# AWS Copilot ECS Fargate / EFS

Deploy a simple Nginx server with persistant Storage EFS / Fargate


[Copilot Docs](https://aws.github.io/copilot-cli/)


1. Install AWS Copilot and AWS CLI
2. Run `copilot init`
3. Run `copilot deploy`

If succesfull, you'll get the following message

```bash
  - You can access your service at http://{GENERATEDURL}.{DEFAULT_REGION}.elb.amazonaws.com over the internet.
```

When the stack is deployed, connect to the container with

`copilot svc exec`

Then add the file to the filesystem

```bash
cd /usr/share/nginx/html
echo "Hello world" > index.html
```
