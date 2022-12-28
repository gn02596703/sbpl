# Demo and Visualization file for (x, y, theta) path planning
The demo file here is from SBPL official website </br>
You can check the detail explanation in the page </br>
http://sbpl.net/node/51

# Running the demo

Once you compile the code, you can run it with

```
$ ./xytheta [location of willow cfg file] [location of motion primitives file]
```

In the standard SBPL install, use these files </br>
(By default, the willow cfg comes as a zip, so you have to unzip it first).

```
env_examples/nav3d/willow-25mm-inflated-env.cfg
matlab/mprim/pr2.mprim
```

This will produce two solution files </br>__sol.txt__ </br> __sol.txt.discrete__

This is the planned path plotted using the code (depends on matplotlib and numpy). You can run this code with

```
python visualize.py willow-25mm-inflated-env.cfg sol.txt.discrete
```