# To run this image:

docker run -it --net=host marcolarosa/ubuntu-xenial-firefox

Note that it's expecting to connect to http://localhost:8080 (that's where your karma server should be running) in order to enslave it for tests. So - be sure to run `karma start test/karma.conf.js` before runnning this image (assuming karma will listen on 8080).