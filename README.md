# Dragonfly-gem5-simulation
ECE 6150 project

Use this garnet2.0 replace the garnet2.0 in the src/mem/ruby/network/garnet2.0 in the gem5 respository

change list:
set Valiant algorithm in the function XY routing, choose Valiant algorithm by command --routing-algorithm=1
Set a global varible busystate to check the busy situation in the NetworkInterface.cc file. Then refer this varible in the UGAL-H routing function to check the input queue whether it is congestion. If it is congested then choose the Valiant routing otherwise choose the Minimal routing. Use command --routing-algorithm=2 to choose UGAL-H routing algorithm=1

In order to simulate the hypercube and dragonfly, recommend to increase the number of virtual channels by command --vcs-per-vnet=16

The topology folder include the hypercube, mesh and dragonfly three topologies which are used to coamparation in the project.
