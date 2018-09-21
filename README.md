# smollet/tftpd
Docker image with alpine and tftpd

## Build

This image can be built on your local box using this command:

```
docker build -t smollet/tftpd https://github.com/SeanMollet/docker-tftpd.git
```

## Run
To launch and use the container with a given directory:
```
docker run --name tftpd -d -p 69:69/udp -v <PathYouWantToShare>:/tftpboot smollet/tftpd
