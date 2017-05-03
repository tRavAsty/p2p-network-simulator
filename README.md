Simulation of a p2p network using [simpy](https://simpy.readthedocs.org/en/latest/)
Prerequisite
======================
Microsoft Visual C++ 9.0 is required. Get it from [here](http://aka.ms/vcpython27)
graphviz from [here](http://www.graphviz.org/Download..php)

``Python
pip install numpy networkx matplotlib pygraphviz
``

Features
======================
Simulation of 
- connections with bandwidth & latency
- messaging
- bootstrapping
- peer reorganisation based on bandwith & availability
- peer downtimes / disconnects
- network slowdowns

The optional network visualization is based on [Networkx](https://networkx.github.io/documentation/latest/)

Usage
======================
To start the default simulation type ```python run.py```.

Browse and modify the source to model your problem. 

The ```Peer``` class offers to register *services* which are based on the ```BaseService``` class. All registered services are called whenever a ```Message``` is received. Services as well as Peers are simpy-processes. 
