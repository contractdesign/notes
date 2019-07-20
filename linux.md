
# Access Jupyter Remotely from a Chromebook

How to run Jupyter remotely and access it from a Chromebook, based on notes from [https://stharrold.github.io/20151208-ipynb-on-gce-from-chrome.html]

1. In the virtual machine, start Jupyter

   jupyter notebook --ip=0.0.0.0 --port=8888 --no-browser &

2. In the Chromebook, forward port 8888 on the VM to 8888 on the localhost using these additional options,

   -N -L localhost:8888:0.0.0.0:8888

Now you can access jupyter from a webbrowser from http://localhost:8888


