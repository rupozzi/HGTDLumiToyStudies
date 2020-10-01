# HGTDLumiToyStudies
Boilerplate for toy simulation studies of luminosity measurements with the HGTD detector at the ATLAS experiment

# How to use this
This repository contains a starting point for how to use the `ROOT` library from `python` in a jupyter notebook. There are two main options for doing this:
* install jupyter notebook directly on your own computer
* use it from a docker container

For the latter option, install docker and put this in your terminal:

```
docker run -v /Users/cohm/Desktop/tmp/HGTDLumiToyStudies/:/work -p 3000:8080 kthatlas/opendatalab:SH1015
```

This will start the docker image `cohm/pyroot-notebook` which contains a jupyter notebook server, and make the path after the `-v` switch (which could e.g. be the path to where you checked out this repository) accessible from inside the notebooks. When starting this image you should get output like this in your terminal:

```
OhmBookPro13:~/Desktop/tmp > docker run -v /Users/cohm/Desktop/tmp/HGTDLumiToyStudies/:/work -p 3000:8080 kthatlas/opendatalab:SH1015
[I 17:57:41.693 NotebookApp] Writing notebook server cookie secret to /root/.local/share/jupyter/runtime/notebook_cookie_secret
[I 17:57:42.040 NotebookApp] Serving notebooks from local directory: /work
[I 17:57:42.040 NotebookApp] The Jupyter Notebook is running at:
[I 17:57:42.040 NotebookApp] http://(2c298ffddff5 or 127.0.0.1):8080/?token=f9f112449b71fc507b51394ce11d9e21c5b4565430581304
[I 17:57:42.040 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[W 17:57:42.041 NotebookApp] No web browser found: could not locate runnable browser.
[C 17:57:42.041 NotebookApp] 
    
    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://(2c298ffddff5 or 127.0.0.1):8080/?token=f9f112449b71fc507b51394ce11d9e21c5b4565430581304
```

If you then open the link `http://127.0.0.1:3000/?token=f9f112449b71fc507b51394ce11d9e21c5b4565430581304` in a browser on your laptop, you can start coding. 

(NB! The port number 8080 in the terminal print-out is changed to 3000 here)
