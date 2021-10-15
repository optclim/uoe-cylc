uoe-cylc
========
Notes and simple workflows for figuring out how to run [cylc 8](https://cylc.github.io/cylc-doc/latest/html/index.html) on our machines.

Installation
------------
 * install into a conda python3 environment 
 ```conda install cylc-flow```
 
Setup
-----

Running a Workflow
------------------
 1. create `~/cylc-src` directory which holds the source for any workflow. I use a symbolic link to my actual source directory.
 2. install the workflow using, eg
 ```cylc install hello```
 3. validate it
 ```cylc validate hello/runN```
 4. run it
  ```cylc run hello/runN```
  output is in `~/cylc-run/hello/runN/log/job/1/hello/NN/`
