# speedus-ubuntu
Ubuntu image with speedus solution for high-performance communications. Check us out at [our website](http://torusware.com/).
![speedus logo](http://torusware.com/ingenyus/images/logowebtorus.png "Torusware Speedus")

Speedus is your communications highway:

- Accelerates communications in the cloud and corporate IT systems
- Faster applications provide businesses with higher competitive advantages while reducing their IT bill
- 100% nonintrusive software solution which takes full advantage of the underlying hardware

In this container we provide a built-in communication tests, Netpipe. Just execute:

    NPtcp &
    NPtcp -h localhost

For getting the baseline. To perform the test with our solution:

    speedus NPtcp &
    speedus NPtcp -h localhost

As you can see, using speedus is really easy and non-intrusive, just type `speedus` before your application:

    speedus /path/to/the/program [parameters]

If you need more information, you can check the README file inside the container or contact us at <info@torusware.com>
