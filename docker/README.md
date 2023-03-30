# Using image with Docker agent template

Make sure the Docker socket is available to Jenkins. This might not be given if you, for example, run your Jenkins instance in a Docker container.

This image can be used to build and deploy Docker containers with your Jenkins pipeline. It is configured as Docker-out-of-Docker. If you want more information about Docker-in-Docker vs. Docker-out-of-Docker you can look [here](http://tdongsi.github.io/blog/2017/04/23/docker-out-of-docker/).

| Key                       | Value                                                                    |
| ------------------------- | ------------------------------------------------------------------------ |
| User                      | `root`                                                                   |
| Mounts                    | `type=bind,source=/var/run/docker.sock,destination=/var/run/docker.sock` |
| Remote File System Root   | `/`                                                                      |
| Connect method            | `Attach Docker container`                                                |
| User (for Connect method) | `root`                                                                   |

