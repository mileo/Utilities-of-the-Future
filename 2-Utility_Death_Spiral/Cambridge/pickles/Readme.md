
1. buildings.p

This is a Python pickle file that when loaded yields a list of building instances. The list contains an object instance for each buildings in our data set. This is the buildings as they are initialized, but without their neighbors listed. That information is contained in the neighDict.p file, which is also loaded by the program. Together, these two pickle files allow us to operate independently of ArcGIS for development purposes.

2. neighDict.p

"neighborhood dictionary". The .p extension indicates that this is a Python pickle file. This is a binary format. The file holds a Python dictionary in which the keys are the building IDs in the
data set and the values are lists of neighbors, where a neighbor is indicated by a building ID.  The Python code loads this file and translates it into a usable dictionary during setup.

3. prosumers.p

This file contains prosumer data created by solar_pv_init.py and is updated by doit function to include prosumers who adopt solar at every tick. 



```
 Copyright KAPSARC. Open source MIT License.
```