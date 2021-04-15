<!-- DO NOT EDIT THIS FILE MANUALLY  -->
<!-- Please read the https://github.com/linuxserver/docker-boinc/blob/master/.github/CONTRIBUTING.md -->

[![linuxserver.io](https://raw.githubusercontent.com/linuxserver/docker-templates/master/linuxserver.io/img/linuxserver_medium.png)](https://linuxserver.io)

[![Blog](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Blog)](https://blog.linuxserver.io "all the things you can do with our containers including How-To guides, opinions and much more!")
[![Discord](https://img.shields.io/discord/354974912613449730.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Discord&logo=discord)](https://discord.gg/YWrKVTn "realtime support / chat with the community and the team.")
[![Discourse](https://img.shields.io/discourse/https/discourse.linuxserver.io/topics.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=discourse)](https://discourse.linuxserver.io "post on our community forum.")
[![Fleet](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=Fleet)](https://fleet.linuxserver.io "an online web interface which displays all of our maintained images.")
[![GitHub](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub&logo=github)](https://github.com/linuxserver "view the source for all of our repositories.")
[![Open Collective](https://img.shields.io/opencollective/all/linuxserver.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=Supporters&logo=open%20collective)](https://opencollective.com/linuxserver "please consider helping us by either donating or contributing to our budget")

The [LinuxServer.io](https://linuxserver.io) team brings you another container release featuring:

* regular and timely application updates
* easy user mappings (PGID, PUID)
* custom base image with s6 overlay
* weekly base OS updates with common layers across the entire LinuxServer.io ecosystem to minimise space usage, down time and bandwidth
* regular security updates

Find us at:

* [Blog](https://blog.linuxserver.io) - all the things you can do with our containers including How-To guides, opinions and much more!
* [Discord](https://discord.gg/YWrKVTn) - realtime support / chat with the community and the team.
* [Discourse](https://discourse.linuxserver.io) - post on our community forum.
* [Fleet](https://fleet.linuxserver.io) - an online web interface which displays all of our maintained images.
* [GitHub](https://github.com/linuxserver) - view the source for all of our repositories.
* [Open Collective](https://opencollective.com/linuxserver) - please consider helping us by either donating or contributing to our budget

# [linuxserver/boinc](https://github.com/linuxserver/docker-boinc)

[![GitHub Stars](https://img.shields.io/github/stars/linuxserver/docker-boinc.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-boinc)
[![GitHub Release](https://img.shields.io/github/release/linuxserver/docker-boinc.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/linuxserver/docker-boinc/releases)
[![GitHub Package Repository](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitHub%20Package&logo=github)](https://github.com/linuxserver/docker-boinc/packages)
[![GitLab Container Registry](https://img.shields.io/static/v1.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=linuxserver.io&message=GitLab%20Registry&logo=gitlab)](https://gitlab.com/linuxserver.io/docker-boinc/container_registry)
[![MicroBadger Layers](https://img.shields.io/microbadger/layers/linuxserver/boinc.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge)](https://microbadger.com/images/linuxserver/boinc "Get your own version badge on microbadger.com")
[![Docker Pulls](https://img.shields.io/docker/pulls/linuxserver/boinc.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=pulls&logo=docker)](https://hub.docker.com/r/linuxserver/boinc)
[![Docker Stars](https://img.shields.io/docker/stars/linuxserver/boinc.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=stars&logo=docker)](https://hub.docker.com/r/linuxserver/boinc)
[![Jenkins Build](https://img.shields.io/jenkins/build?labelColor=555555&logoColor=ffffff&style=for-the-badge&jobUrl=https%3A%2F%2Fci.linuxserver.io%2Fjob%2FDocker-Pipeline-Builders%2Fjob%2Fdocker-boinc%2Fjob%2Fmaster%2F&logo=jenkins)](https://ci.linuxserver.io/job/Docker-Pipeline-Builders/job/docker-boinc/job/master/)
[![LSIO CI](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=CI&query=CI&url=https%3A%2F%2Fci-tests.linuxserver.io%2Flinuxserver%2Fboinc%2Flatest%2Fci-status.yml)](https://ci-tests.linuxserver.io/linuxserver/boinc/latest/index.html)

[BOINC](https://boinc.berkeley.edu/) is a platform for high-throughput computing on a large scale (thousands or millions of computers). It can be used for volunteer computing (using consumer devices) or grid computing (using organizational resources). It supports virtualized, parallel, and GPU-based applications.
[![boinc](https://raw.githubusercontent.com/BOINC/boinc/master/doc/logo/boinc_logo_black.jpg)](https://boinc.berkeley.edu/)

## Supported Architectures

Our images support multiple architectures such as `x86-64`, `arm64` and `armhf`. We utilise the docker manifest for multi-platform awareness. More information is available from docker [here](https://github.com/docker/distribution/blob/master/docs/spec/manifest-v2-2.md#manifest-list) and our announcement [here](https://blog.linuxserver.io/2019/02/21/the-lsio-pipeline-project/).

Simply pulling `ghcr.io/linuxserver/boinc` should retrieve the correct image for your arch, but you can also pull specific arch images via tags.

The architectures supported by this image are:

| Architecture | Tag |
| :----: | --- |
| x86-64 | latest |
| arm64 | arm64v8-latest |
| armhf | arm32v7-latest |

## Application Setup

This image sets up the BOINC client and manager and makes its interface available via Guacamole server in the browser. The interface is available at `http://your-ip:8080`.

By default, there is no password set for the main gui. Optional environment variable `PASSWORD` will allow setting a password for the user `abc`.

You can access advanced features of the Guacamole remote desktop using `ctrl`+`alt`+`shift` enabling you to use remote copy/paste and different languages.

It is recommended to switch to `Advanced View` in the top menu, because the `Computing Preferences` don't seem to be displayed in `Simple View`.

Sometimes, the pop-up windows may open in a tiny box in the upper left corner of the screen. When that happens, you can find the corner and resize them.

## GPU Hardware Acceleration

### Intel

Hardware acceleration users for Intel Quicksync will need to mount their /dev/dri video device inside of the container by passing the following command when running or creating the container:
```--device=/dev/dri:/dev/dri```
We will automatically ensure the abc user inside of the container has the proper permissions to access this device.

### Nvidia

Hardware acceleration users for Nvidia will need to install the container runtime provided by Nvidia on their host, instructions can be found here:
https://github.com/NVIDIA/nvidia-docker
We automatically add the necessary environment variable that will utilise all the features available on a GPU on the host. Once nvidia-docker is installed on your host you will need to re/create the docker container with the nvidia container runtime `--runtime=nvidia` and add an environment variable `-e NVIDIA_VISIBLE_DEVICES=all` (can also be set to a specific gpu's UUID, this can be discovered by running `nvidia-smi --query-gpu=gpu_name,gpu_uuid --format=csv` ). NVIDIA automatically mounts the GPU and drivers from your host into the BOINC docker container.

## Usage

Here are some example snippets to help you get started creating a container.

### docker-compose ([recommended](https://docs.linuxserver.io/general/docker-compose))

Compatible with docker-compose v2 schemas.

```yaml
---
version: "2.1"
services:
  boinc:
    image: ghcr.io/linuxserver/boinc
    container_name: boinc
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=Europe/London
      - PASSWORD= #optional
    volumes:
      - /path/to/data:/config
    ports:
      - 8080:8080
    devices:
      - /dev/dri:/dev/dri #optional
    restart: unless-stopped
```

### docker cli

```bash
docker run -d \
  --name=boinc \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Europe/London \
  -e PASSWORD= `#optional` \
  -p 8080:8080 \
  -v /path/to/data:/config \
  --device /dev/dri:/dev/dri `#optional` \
  --restart unless-stopped \
  ghcr.io/linuxserver/boinc
```

## Parameters

Container images are configured using parameters passed at runtime (such as those above). These parameters are separated by a colon and indicate `<external>:<internal>` respectively. For example, `-p 8080:80` would expose port `80` from inside the container to be accessible from the host's IP on port `8080` outside the container.

| Parameter | Function |
| :----: | --- |
| `-p 8080` | Boinc desktop gui. |
| `-e PUID=1000` | for UserID - see below for explanation |
| `-e PGID=1000` | for GroupID - see below for explanation |
| `-e TZ=Europe/London` | Specify a timezone to use EG Europe/London. |
| `-e PASSWORD=` | Optionally set a password for the gui. |
| `-v /config` | Where BOINC should store its database and config. |
| `--device /dev/dri` | Only needed if you want to use your Intel GPU (vaapi). |

## Environment variables from files (Docker secrets)

You can set any environment variable from a file by using a special prepend `FILE__`.

As an example:

```bash
-e FILE__PASSWORD=/run/secrets/mysecretpassword
```

Will set the environment variable `PASSWORD` based on the contents of the `/run/secrets/mysecretpassword` file.

## Umask for running applications

For all of our images we provide the ability to override the default umask settings for services started within the containers using the optional `-e UMASK=022` setting.
Keep in mind umask is not chmod it subtracts from permissions based on it's value it does not add. Please read up [here](https://en.wikipedia.org/wiki/Umask) before asking for support.

## User / Group Identifiers

When using volumes (`-v` flags) permissions issues can arise between the host OS and the container, we avoid this issue by allowing you to specify the user `PUID` and group `PGID`.

Ensure any volume directories on the host are owned by the same user you specify and any permissions issues will vanish like magic.

In this instance `PUID=1000` and `PGID=1000`, to find yours use `id user` as below:

```bash
  $ id username
    uid=1000(dockeruser) gid=1000(dockergroup) groups=1000(dockergroup)
```

## Docker Mods

[![Docker Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=boinc&query=%24.mods%5B%27boinc%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=boinc "view available mods for this container.") [![Docker Universal Mods](https://img.shields.io/badge/dynamic/yaml?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&label=universal&query=%24.mods%5B%27universal%27%5D.mod_count&url=https%3A%2F%2Fraw.githubusercontent.com%2Flinuxserver%2Fdocker-mods%2Fmaster%2Fmod-list.yml)](https://mods.linuxserver.io/?mod=universal "view available universal mods.")

We publish various [Docker Mods](https://github.com/linuxserver/docker-mods) to enable additional functionality within the containers. The list of Mods available for this image (if any) as well as universal mods that can be applied to any one of our images can be accessed via the dynamic badges above.

## Support Info

* Shell access whilst the container is running: `docker exec -it boinc /bin/bash`
* To monitor the logs of the container in realtime: `docker logs -f boinc`
* container version number
  * `docker inspect -f '{{ index .Config.Labels "build_version" }}' boinc`
* image version number
  * `docker inspect -f '{{ index .Config.Labels "build_version" }}' ghcr.io/linuxserver/boinc`

## Updating Info

Most of our images are static, versioned, and require an image update and container recreation to update the app inside. With some exceptions (ie. nextcloud, plex), we do not recommend or support updating apps inside the container. Please consult the [Application Setup](#application-setup) section above to see if it is recommended for the image.

Below are the instructions for updating containers:

### Via Docker Compose

* Update all images: `docker-compose pull`
  * or update a single image: `docker-compose pull boinc`
* Let compose update all containers as necessary: `docker-compose up -d`
  * or update a single container: `docker-compose up -d boinc`
* You can also remove the old dangling images: `docker image prune`

### Via Docker Run

* Update the image: `docker pull ghcr.io/linuxserver/boinc`
* Stop the running container: `docker stop boinc`
* Delete the container: `docker rm boinc`
* Recreate a new container with the same docker run parameters as instructed above (if mapped correctly to a host folder, your `/config` folder and settings will be preserved)
* You can also remove the old dangling images: `docker image prune`

### Via Watchtower auto-updater (only use if you don't remember the original parameters)

* Pull the latest image at its tag and replace it with the same env variables in one run:

  ```bash
  docker run --rm \
  -v /var/run/docker.sock:/var/run/docker.sock \
  containrrr/watchtower \
  --run-once boinc
  ```

* You can also remove the old dangling images: `docker image prune`

**Note:** We do not endorse the use of Watchtower as a solution to automated updates of existing Docker containers. In fact we generally discourage automated updates. However, this is a useful tool for one-time manual updates of containers where you have forgotten the original parameters. In the long term, we highly recommend using [Docker Compose](https://docs.linuxserver.io/general/docker-compose).

### Image Update Notifications - Diun (Docker Image Update Notifier)

* We recommend [Diun](https://crazymax.dev/diun/) for update notifications. Other tools that automatically update containers unattended are not recommended or supported.

## Building locally

If you want to make local modifications to these images for development purposes or just to customize the logic:

```bash
git clone https://github.com/linuxserver/docker-boinc.git
cd docker-boinc
docker build \
  --no-cache \
  --pull \
  -t ghcr.io/linuxserver/boinc:latest .
```

The ARM variants can be built on x86_64 hardware using `multiarch/qemu-user-static`

```bash
docker run --rm --privileged multiarch/qemu-user-static:register --reset
```

Once registered you can define the dockerfile to use with `-f Dockerfile.aarch64`.

## Versions

* **23.03.21:** - Rebase to rdesktop-web baseimage. Deprecate `GUAC_USER` and `GUAC_PASS` env vars. Existing users can set the new var `PASSWORD` for the user `abc`.
* **01.04.20:** - Install boinc from ppa.
* **17.03.20:** - Add armhf and aarch64 builds and switch to multi-arch image.
* **16.03.20:** - Clean up old pid files.
* **15.03.20:** - Initial release.
