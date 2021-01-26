# Introduction

This is a quick approach to Apache Airflow with Celery using Linux.

# TL;DR

First, you need to make the file **entrypoint.sh** in **script** readable, writeable and executable. So, run the following command:

```shell
chmod 775 script/entrypoint.sh
```

Then, run the file **build_docker_image.sh**

```shell
source build_docker_image.sh
```

Then, run the file **run_docker_compose.sh**

```shell
source run_docker_compose.sh
```

Set the number of Celery workers with

```shell
# If you want to modify the number of workers,
# change the end of scale_worker.sh file. E.g.,
# 'worker=3' to 'worker=1'
source scale_worker.sh
```

Finally, if you want to stop all docker-composer containers

```shell
source stop_docker_compose.sh
```


# Old README

The old **README** file from puckel can be found [here](https://github.com/puckel/docker-airflow)
