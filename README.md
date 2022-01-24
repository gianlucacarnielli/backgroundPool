# Offloading Callback Execution to a Background Pool

## Overview
This demo shows how to use "backgroundPool" within App Designer to separate a callback execution from the app's thread.

## How to run this demo
To see the use of "backgroundPool" proceed as follows:
* Run the "Parallel App" (e.g., via the project shortcut);
* Press the "Start Simulation" button;
* Wait a couple of seconds;
* Press the "Generate Random Data" button.

**In this case, the table data is updated in a separate thread and the simulation does not pause.**

To compare with a case where the callback is not offloaded to a new thread follow the steps below:
* Run the "Series App" (e.g., via the project shortcut);
* Press the "Start Simulation" button;
* Wait a couple of seconds;
* Press the "Generate Random Data" button.

**In this other case, updating the table will temporarily stop the simulation execution since the callback is executed within the app.**

The code for boths apps can be inspected in App Designer.

## Required Products
* MATLAB®

Copyright 2022 The MathWorks, Inc.
