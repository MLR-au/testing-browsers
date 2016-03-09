# Real browsers inside a docker container for karma tests


Assuming you use karma for running your unit tests and assuming it runs on 8080 when you start it, you can use these docker containers to fire up a browser which connects to karma and gets enslaved for the purpose of running the tests.

## Invocation
- Start karma: `karma start test/karma.conf.js`
- Fire up one or more browsers with something like: `docker run -it --net=host {IMAGE}` (assuming the image has an entrypoint | command which starts the browser and points it at http://localhost:8080).

## Firefox
Firefox inside latest Ubuntu (at time of creation: Ubuntu Xenial). 

## Chrome
Yet to get it working inside a docker container so if anyone knows how to get chrome going please reach out!