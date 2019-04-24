![speedus logo](http://dl.torusware.com/images/speedus_small.jpg "Torusware Speedus")
![ubuntu logo](https://assets.ubuntu.com/v1/4e9b777c-ubuntu-orange-on-white.gif "Ubuntu")
# Speedus Plug&Run for Ubuntu
Ubuntu image with speedus solution for high-performance communications. Check us out at [our website](https://bit.ly/1MKxCuh).

Speedus is your communications highway:

- Accelerates communications in the cloud and corporate IT systems
- Faster applications provide businesses with higher competitive advantages while reducing their IT bill
- 100% nonintrusive software solution which takes full advantage of the underlying hardware

# Supported tags and respective `Dockerfile` link
Each tag corresponds to the tag of the Ubuntu base image:

- [`bionic`](https://github.com/torusware/speedus-ubuntu/tree/master/bionic "xenial Dockerfile"), [`latest`](https://github.com/torusware/speedus-ubuntu/tree/master/bionic "latest Dockerfile")
- [`xenial`](https://github.com/torusware/speedus-ubuntu/tree/master/xenial "xenial Dockerfile")
- [`trusty`](https://github.com/torusware/speedus-ubuntu/tree/master/trusty "trusty Dockerfile")
- [`precise`](https://github.com/torusware/speedus-ubuntu/tree/master/precise "precise Dockerfile")

# Launching instructions
In order to run a container with our image, execute:
```bash
sudo docker run -ti torusware/speedus-ubuntu
```

This will launch a `bash` shell where you can execute whatever program you want.

In this image we provide a built-in communication tests, Netpipe. Execute the next lines in order to obtain the baseline performance:
```bash
NPtcp &
NPtcp -h localhost
```

To run the same test using Speedus:
```bash
speedus NPtcp &
speedus NPtcp -h localhost
```

As you can see, using Speedus is really easy and non-intrusive, just type `speedus` before your application:
```bash
speedus /path/to/the/program [parameters]
```

If you need more information, you can check the README file inside the container or contact us at **info@torusware.com**

# Check our other images in the Docker Hub

- [Speedus Plug&Run for Redis](https://registry.hub.docker.com/u/torusware/speedus-redis/)
- [Speedus Plug&Run for CentOS](https://registry.hub.docker.com/u/torusware/speedus-centos/)
- [Speedus Plug&Run for MongoDB](https://registry.hub.docker.com/u/torusware/speedus-mongo/)
- [Speedus Plug&Run for YCSB](https://registry.hub.docker.com/u/torusware/speedus-ycsb/)

# Example Use Cases

- [Optimizing communications between Docker containers](https://bit.ly/1IZdodU)
- [Increasing performace of a Redis Docker container in Amazon Web Services](https://bit.ly/1KsVBJW)
- [Increasing performace of a MongoDB Docker container in Azure](https://bit.ly/1KGHxNW)
