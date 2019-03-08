# Jupyter SciPy + NLTK

Now you can go ahead and NLP away

## Main instructions

Run on any Unix-based OS:

```
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v ${PWD}:/home/jovyan/work -v "$PWD"/data:/home/jovyan/nltk_data jtemporal/nltkjupyter
```

Run on windows:

```
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v ${PWD}:/home/jovyan/work -v ${PWD}\data:/home/jovyan/nltk_data jtemporal/nltkjupyter
```

To Build
```
docker build -t jtemporal/nltkjupyter .
```

## Using this image

### volumes

The first volume up there (`${PWD}:/home/jovyan/work`) makes the workspace for the notebooks, whereas the second one `(`${PWD}\data:/home/jovyan/nltk_data`) makes sure that you don't have to download the data all the time.

### data

Here my data directory is called `data/` (I'm not very good one naming). 

## Jupyter Docker stacks

If you have more questions about running jupyter with docker, maybe the [jupyter docker stacks documentation](http://jupyter-docker-stacks.readthedocs.io/).
