# HGTDLumiToyStudies
Boilerplate for toy simulation studies of luminosity measurements with the HGTD detector at the ATLAS experiment

# How to use this
This repository contains a starting point for how to use the `ROOT` library from `python` in a jupyter notebook. You can either install jupyter notebook directly on your own computer, or use it from a docker container, e.g. like this:

```
docker run -v /Users/cohm/Desktop/tmp/HGTDLumiToyStudies/:/work -p 3000:8080 cohm/pyroot-notebook
```
This will start the docker image `cohm/pyroot-notebook` which contains a jupyter notebook server, and make the path after the `-v` switch (which could e.g. be the path to where you checked out this repository) accessible from inside the notebooks. 
