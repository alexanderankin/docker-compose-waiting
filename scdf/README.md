# scdf docker-compose.yaml

This exercise was done to confirm the viability of a method to get rid of a
dependency in SCDF.

The file itself is taken from these docs: https://dataflow.spring.io/docs/installation/local/docker/

which provide the following instructions:

```
wget -O docker-compose.yml https://raw.githubusercontent.com/spring-cloud/spring-cloud-dataflow/v2.9.1/src/docker-compose/docker-compose.yml; \
DATAFLOW_VERSION=2.9.2 SKIPPER_VERSION=2.8.2 \
docker-compose up
```

the file `original.yaml` in this repository contains the contents of this url
at the time of writing:

```
https://raw.githubusercontent.com/spring-cloud/spring-cloud-dataflow/v2.9.1/src/docker-compose/docker-compose.yml
```

the file `docker-compose.yaml` in this directory contains the amended file
without `apt-get update` on startup (!!) [1][1].

[1]: https://arstechnica.com/tech-policy/2021/02/comcast-responds-to-pressure-cancels-data-cap-in-northeast-us-until-2022/
