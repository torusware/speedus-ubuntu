![speedus logo](http://dl.torusware.com/images/speedus_small.jpg "Torusware Speedus")
![ubuntu logo](http://www.gandotech.net/wp-content/uploads/2014/06/Ubuntu.png "Ubuntu")
# Speedus Plug&Run Lite for Ubuntu
Ubuntu image with Torusware Speedus Plug&Run Lite solution for high-performance communications. Check us out at [our website](http://torusware.com/).

Speedus is your communications highway:

- Accelerates communications in the cloud and corporate IT systems
- Faster applications provide businesses with higher competitive advantages while reducing their IT bill
- 100% nonintrusive software solution which takes full advantage of the underlying hardware

#Supported tags and respective `Dockerfile` link
Each tag corresponds to the tag of the ubuntu base image:

- [`trusty`](https://github.com/torusware/speedus-ubuntu/tree/master/trusty "trusty Dockerfile"), [`latest`](https://github.com/torusware/speedus-ubuntu/tree/master/trusty "latest Dockerfile")
- [`precise`](https://github.com/torusware/speedus-ubuntu/tree/master/precise "precise Dockerfile")

#Launching instructions
In order to run a container with our image, execute:

    sudo docker run -ti torusware/speedus-ubuntu

This will launch a `bash` shell where you can execute whatever program you want.

In this image we provide a built-in communication tests, [NetPIPE](http://bitspjoule.org/netpipe/). In order to obtain the baseline performance:

    NPtcp &
    NPtcp -h localhost

Now, compare these results with the same test running with Speedus:

    speedus NPtcp &
    speedus NPtcp -h localhost

As you can see, using speedus is really easy and non-intrusive, just type `speedus` before your application:

    speedus /path/to/the/program [parameters]

If you need more information, you can check the README file inside the container or contact us at <info@torusware.com>

#Check our other images in the Docker Hub

- [speedus-centos image](https://registry.hub.docker.com/u/torusware/speedus-centos/ "Speedus Plug&Run Lite for CentOS")
- [speedus-redis image](https://registry.hub.docker.com/u/torusware/speedus-redis/ "Speedus Plug&Run Lite for Redis")
- [speedus-mongo image](https://registry.hub.docker.com/u/torusware/speedus-mongo/ "Speedus Plug&Run Lite for MongoDB")

#Example Use Case

- [Optimizing communications between Docker containers](http://blog.torusware.com/2015/04/optimizing-communications-between.html "Optimizing communications between Docker containers")
- [Increasing performace of a MongoDB Docker container in Azure](http://blog.torusware.com/2015/05/increasing-performace-of-mongodb-docker.html "Increasing performace of a MongoDB Docker container in Azure")
