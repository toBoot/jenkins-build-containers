# Using image with Docker Agent Template

Make shure the Docker socket is available to Jenkins. This might not be given if you, for example, run your Jenkins instance in a Docker Container.

| Key                       | Value                                                                    |
| ------------------------- | ------------------------------------------------------------------------ |
| User                      | `root`                                                                     |
| Mounts                    | `type=bind,source=/var/run/docker.sock,destination=/var/run/docker.sock` |
| Remote File System Root   | `/`                                                                      |
| Connect method            | `Attach Docker container`                                                |
| User (for Connect method) | `root`                                                                   |

