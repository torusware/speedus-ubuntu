![speedus logo](http://dl.torusware.com/images/speedus_small.jpg "Torusware Speedus")
![ubuntu logo](http://design.ubuntu.com/wp-content/uploads/ubuntu-orange-on-white.gif "Ubuntu")
# Speedus Plug&Run Lite for Ubuntu
Ubuntu image with speedus solution for high-performance communications. Check us out at [our website](https://bit.ly/1MKxCuh).

Speedus is your communications highway:

- Accelerates communications in the cloud and corporate IT systems
- Faster applications provide businesses with higher competitive advantages while reducing their IT bill
- 100% nonintrusive software solution which takes full advantage of the underlying hardware

# Supported tags and respective `Dockerfile` link
Each tag corresponds to the tag of the ubuntu base image:

- [`trusty`](https://github.com/torusware/speedus-ubuntu/tree/master/trusty "trusty Dockerfile"), [`latest`](https://github.com/torusware/speedus-ubuntu/tree/master/trusty "latest Dockerfile")
- [`precise`](https://github.com/torusware/speedus-ubuntu/tree/master/precise "precise Dockerfile")

# Launching instructions
In order to run a container with our image, execute:
```bash
sudo docker run -ti torusware/speedus-ubuntu
```

This will launch a `bash` shell where you can execute whatever program you want.

In this image we provide a built-in communication tests, Netpipe. Just execute:
```bash
NPtcp &
NPtcp -h localhost
```

For getting the baseline. To perform the test with our solution:
```bash
speedus NPtcp &
speedus NPtcp -h localhost
```

As you can see, using speedus is really easy and non-intrusive, just type `speedus` before your application:
```bash
speedus /path/to/the/program [parameters]
```

If you need more information, you can check the README file inside the container or contact us at **info@torusware.com**

# Check our other images in the Docker Hub

- [Speedus Plug&Run Lite for Redis](https://registry.hub.docker.com/u/torusware/speedus-redis/)
- [Speedus Plug&Run Lite for CentOS](https://registry.hub.docker.com/u/torusware/speedus-centos/)
- [Speedus Plug&Run Lite for MongoDB](https://registry.hub.docker.com/u/torusware/speedus-mongo/)
- [Speedus Plug&Run Lite for YCSB](https://registry.hub.docker.com/u/torusware/speedus-ycsb/)

# Example Use Cases

- [Optimizing communications between Docker containers](https://bit.ly/1IZdodU)
- [Increasing performace of a Redis Docker container in Amazon Web Services](https://bit.ly/1KsVBJW)
- [Increasing performace of a MongoDB Docker container in Azure](https://bit.ly/1LgUzDV)

