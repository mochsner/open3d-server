In order to make 3D models from open3d.org accessible on the web, there's 2 ways documented on version 0.13.0: [**standalone**](http://www.open3d.org/docs/release/tutorial/visualization/web_visualizer.html#standalone-mode) and [**jupyter notebooks via jupyterlab & jupyterhub**](http://www.open3d.org/docs/release/tutorial/visualization/web_visualizer.html#jupyter-mode). 


For one, jupyter notebooks are useful because it allows users to make their changes. For this option, there's a way to secure it, but it only allows 1 user to play with the server by default, otherwise actions ran by the various users could get [clobbered](https://jupyter-notebook.readthedocs.io/en/stable/public_server.html). The solution to this is to use [Jupyterhub](https://jupyterhub.readthedocs.io/en/latest/), which can get fairly complex. See below diagram for what this "hub" looks like:
![](2021-08-23-15-44-52.png)

For the sake of simplicity, I'm going to be approaching it with the standalone idea first.