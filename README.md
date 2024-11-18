# WISHBONE PIPELINE SLAVE
### Wishbone Pipeline slave to Analog Devices uP interface

![image](docs/manual/img/AFRL.png)

---

   author: Jay Convertino   
   
   date: 2024.02.19
   
   details: Interface analog devices uP interface devices to Wishbone Pipeline bus
   
   license: MIT   
   
---

### Version
#### Current
  - V1.0.0 - initial release

#### Previous
  - none

### DOCUMENTATION
  For detailed usage information, please navigate to one of the following sources. They are the same, just in a different format.

  - [up_wishbone_pipeline.pdf](docs/manual/up_wishbone_pipeline.pdf)
  - [github page](https://johnathan-convertino-afrl.github.io/up_wishbone_pipeline/)

### DEPENDENCIES
#### Build

  - AFRL:utility:helper:1.0.0
  
#### Simulation

  - AFRL:simulation:axis_stimulator

### PARAMETERS

* ADDRESS_WIDTH : Bit width of the address bus.
* BUS_WIDTH     : Bus width in number of bytes.

### COMPONENTS
#### SRC

* wishbone_slave.v
  
#### TB

* tb_wishbone_slave.v
  
### FUSESOC

* fusesoc_info.core created.
* Simulation uses icarus to run data through the core.

#### Targets

* RUN WITH: (fusesoc run --target=sim VENDER:CORE:NAME:VERSION)
  - default (for IP integration builds)
  - sim
