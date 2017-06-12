# mysilen

a painless docker/moby for studying machine-learning (non-gpu)

# usage

## making a docker container
```
$ docker run --name yoursilen -d -p 8888:8888 -it mysilen bash
```

## diving in
```
$ docker exec -it yoursilen bash
```

## running jupyter-notebook

in your container's bash:
```
$ jupyter-notebook --ip=0.0.0.0 --allow-root --no-browser
```

output:
> ...
> [I 17:12:17.060 NotebookApp] The Jupyter Notebook is running at: http://0.0.0.0:8888/?token=631a47a1c6d079165565461caa2e292f01e44cf680dbbda9
> ...

in your local browser:
> http://localhost:8888/?token=631a47a1c6d079165565461caa2e292f01e44cf680dbbda9
