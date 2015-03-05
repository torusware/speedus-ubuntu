![speedus logo](http://torusware.com/ingenyus/images/logowebtorus.png "Torusware Speedus")
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
