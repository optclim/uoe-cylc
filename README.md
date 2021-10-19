uoe-cylc
========
Notes and simple workflows for figuring out how to run [cylc 8](https://cylc.github.io/cylc-doc/latest/html/index.html) on our machines.

Installation
------------
 * install into a conda python3 environment 
 ```conda install cylc-flow```
 
Setup
-----
1. copy the [global.cylc](global.cylc) into `~/.cylc/flow/`. I use a symbolic link for that.

Running a Workflow
------------------
 1. create `~/cylc-src` directory which holds the source for any workflow. I use a symbolic link to my actual source directory.
 2. install the workflow using without the run name, eg
 ```cylc install hello --no-run-name```
 3. validate it
 ```cylc validate hello```
 4. run it
  ```cylc run hello```
  output is in `~/cylc-run/hello/log/job/1/hello/NN/`
 5. check progress ```cylc tui hello```
  
