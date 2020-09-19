## Docker builds
Build YaakTech OpenCV Image from [`docker`](https://github.com/yaak-ai/opencv/tree/docker) branch.

### Table

- [Prerequisites](https://github.com/yaak-ai/opencv/tree/docker/docker#prerequisites)
- Build OpenCV
  - [CPU](https://github.com/yaak-ai/opencv/tree/docker/docker#opencv)
  - GPU (TODO)
- [Push Image to DockerHub](https://github.com/yaak-ai/opencv/tree/docker/docker#dockerhub)

#### Prerequisites
  1. Install docker for [Mac OS](https://www.docker.com/products/docker-desktop) or [Linux](https://docs.docker.com/engine/install/ubuntu/).
  2. `sudo usermod -aG docker $USER`
  3. Logout and Login again (for Linux)

#### Docker Compose

  Follow steps outlined [here](https://github.com/yaak-ai/service-calibration/blob/master/scripts/install_docker.sh)

#### OpenCV
```
  docker-compose -f docker/ubuntu/docker-compose.yml build opencv
```

#### DockerHub
```
  docker-compose -f docker/ubuntu/docker-compose.yml push opencv
```
