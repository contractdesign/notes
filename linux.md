# Notes

## tar

    tar cvzf dir.tar.gz dir/    # tar a directory
    tar xvzf dir.tar.gz         # untar it

## makefile

    make -qp                    # list rules

## Jupyter

How to run Jupyter remotely and access it from a Chromebook, based on notes from
[https://stharrold.github.io/20151208-ipynb-on-gce-from-chrome.html](ipyb from chrome) 

1. In the virtual machine, start Jupyter
```
    jupyter notebook --ip=0.0.0.0 --port=8888 --no-browser &
```

2. In the Chromebook, forward port 8888 on the VM to 8888 on the localhost using these additional options,
```
    ssh -N -L localhost:8888:0.0.0.0:8888
```
Now you can access jupyter from a webbrowser from http://localhost:8888


