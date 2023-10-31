# 2023
https://fusionauth.io/docs/v1/tech/developer-guide/api-gateways/kong-gateway
## Get Kong 
* https://docs.konghq.com/gateway/3.4.x/get-started/
```bash
curl -Ls https://get.konghq.com/quickstart | bash
```
### Access Kong Manager - GUI
While the rest of this guide demonstrates configuring Kong Gateway using the Admin API, you can also use Kong Manager to manage your Services, Routes, Plugins, and more. To access Kong Manager, go to the following URL: http://localhost:8002
## Services and Routes 
* https://docs.konghq.com/gateway/3.4.x/get-started/services-and-routes/

# Kong in Docker Compose

This is the official Docker Compose template for [Kong][kong-site-url].

# What is Kong?

You can find the official Docker distribution for Kong at [https://store.docker.com/images/kong](https://store.docker.com/images/kong).

# How to use this template

This Docker Compose template provisions a Kong container with a Postgres database, plus a nginx load-balancer. After running the template, the `nginx-lb` load-balancer will be the entrypoint to Kong.

To run this template execute:

```shell
$ docker-compose up
```

To scale Kong (ie, to three instances) execute:

```shell
$ docker-compose scale kong=3
```

Kong will be available through the `nginx-lb` instance on port `8000`, and `8001`. You can customize the template with your own environment variables or datastore configuration.

Kong's documentation can be found at [https://docs.konghq.com/][kong-docs-url].

## Issues

If you have any problems with or questions about this image, please contact us through a [GitHub issue][github-new-issue].
