Deep Dream Container
====================

This is an example Deep Dream container that runs https://github.com/google/deepdream

This example assumes you know how to run Docker and use IPython Notebook.

This is not an official Google product.

Running the Container
---------------------
To run this container:

    $ docker run -ti -p 8888:8888 saturnism/deepdream

Then you can open the ipython notebook:

    http://localhost:8888/notebooks/dream.ipynb

If you are running Docker Machine on a remote host, make sure you have opened the port
in the firewall settings.

Deep Dream with Your Own Image
------------------------------
To use your own image, you should copy it into a local directory on the Docker host
and then mount it:

    $ docker run -ti -p 8888:8888 -v /myfiles:/deepdream/deepdream/files

You can then refer to the file in IPython Notebook.
