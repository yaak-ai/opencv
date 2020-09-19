## Docker builds
Build YaakTech OpenCV Image from [`docker`](https://github.com/yaak-ai/opencv/tree/docker) branch.

### Table

- Prerequisites
- Build OpenCV
  - CPU
  - GPU (TODO)
- Push Image to DockerHub

### Prerequisites
#### Docker
  1. Install docker for [Mac OS](https://www.docker.com/products/docker-desktop) or [Linux](https://docs.docker.com/engine/install/ubuntu/).
  2. `sudo usermod -aG docker $USER`
  3. Logout and Login again (for Linux)

#### Docker Compose
  1. Follow steps outlined [here](https://github.com/yaak-ai/service-calibration/blob/master/scripts/install_docker.sh)

#### OpenCV
  1. `docker-compose -f docker/ubuntu/docker-compose.yml build opencv`

#### DockerHub
  1. `docker-compose -f docker/ubuntu/docker-compose.yml push opencv`
