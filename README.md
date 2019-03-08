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
