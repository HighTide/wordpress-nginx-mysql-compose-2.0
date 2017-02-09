# wordpress-nginx-mysql-compose-2.0
Modified version of https://github.com/mzsea/docker-compose-wordpress-nginx

Using docker compose to launch wordpress with nginx and php-fpm.
## Installation
You need to have a docker running with:
https://github.com/jwilder/nginx-proxy

You need to add a docker proxy network to your nginx-proxy
```bash
$ docker network create service-proxy
$ docker network connect service-proxy nginx-proxy
```

Clone the repository or download zip and decompression.

```bash
$ git clone https://github.com/KoetseJ/wordpress-nginx-mysql-compose-2.0.git
```

Modify the docker-compose.yml file with your settings!

## Usage

Before run, you can modify profiles with your parameters.
e.g. official image version, ports, mysql password, wordpress version.

The `docker-compose.yml` file using the version 2 syntax, and version 2 files are supported by Compose 1.6.0+ and require a Docker Engine of version 1.10.0+.

Rxecute the following command:

```bash
$ docker-compose up -d
```

Now, you can configure wordpress via URL in a browser and enjoy it.
