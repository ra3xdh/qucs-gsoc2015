## Google Summer of Code (GSOC 2015) ideas list

```
Author: Vadim Kuznetsov
Status: Draft
Created: 22/01/2014
```

### Introduction

Here is the list of our ideas for GSOC-2015. These ideas were contributed by 
our developers.

### Ideas list

#### Qucs-filter extension

**Brief explanation:** Currently we have two passive filter synthesis systems: 
`qucs-filter` and unfinished `qucs-filter-v2`. We want to merge them into one. 
It's need to backport some features from `qucs-filter-v2` to 
`qucs-filter`(Legendre and Blinchikoff filter transfer function 
approximations). See https://github.com/Qucs/qucs/issues/161 . Also we want to 
add Legenedre approximation to `qucs-activefiler` (active filters synthesis 
tool). It's desirable to add inductor coupled resonators topology (see 
schematic) for passive filters. This topology is important for high-power 
output fiters of RF power amplifiers.

![Inductive coupled resonator filter](http://storage4.static.itmages.ru/i/15/0216/h_1424090615_4023764_ea1990efc9.png)

**Expected results :**  New transfer function approximations and filter 
topologies in `qucs-filter`

**Task level :** easy

**Required skills :**  C++, Qt, mathematics,  electronics or electrical 
engineering

**Contact person :**  Vadim Kuznetsov ra3xdh@gmail.com 

#### Extend Qucs components library

**Brief explanation :**  Qucs has not so may components in its system library. 
Especially it concerns Inegrated Circuits (ICs) such as opamps, switching 
circuits, power supply circuits, optocouplers. Transistors (bipolar and FET) 
are also desired. 

It is need to add as many as possible components in Qucs library. 
Components models should be converted from SPICE models that are 
provided in datasheets. Perhaps it's need to implement scripts for auto 
conversion of these models. Especially it concerns opamps.

**Expected results :** More components in Qucs library

**Task level :** easy

**Required skills :** XML, scripting languages (Bash, Python, etc.), SPICE 
models, electronics or electrical engineering 

**Contact person :** Vadim Kuznetsov ra3xdh@gmail.com

#### Add more components with Spice-compatibility

**Brief explanation :** Currently we are performing work on Qucs and other 
SPICE-compatible circuit simulation backends interfacing (Ngspice and Xyce). 
You can find current status of development here on issue tracker: 
https://github.com/Qucs/qucs/issues/181 https://github.com/Qucs/qucs/issues/77 
and on wikipage: 
https://github.com/Qucs/qucs/wiki/QEP%3A-Qucs-schematic-simulation-with-ngspice

It's need to add more spice-compatible components. It's need to implement spice 
netlist builders for them for this purpose. 

**Expected results :** More components in Qucs library

**Task level :** easy

**Required skills :** C++, Qt, SPICE models, electronics or electrical 
engineering 

**Contact person :** Vadim Kuznetsov ra3xdh@gmail.com

#### Qucs library editor

**Brief explanation :** Qucs libraries have XML text format. There is no 
GUI library editor now. It requires open library with text editor and edit it 
manually. You will need to implement Qt-based GUI qucs-tool "Library editor".

**Expected results :** 

Lirary editor should perform the following functions:

1. Edit component name and description 
2. Attach component model from Qucs netlist or schematic
3. Attach Verilog and VHDL models
4. Attach component symbol
4. Attach specific netlist node names to component symbol pins
5. Edit component model or netlist
6. Convert spice model to Qucs model

**Task level :** medium

**Required skills :** C++, Qt, SPICE models, electronics or electrical 
engineering

**Contact person :** Vadim Kuznetsov ra3xdh@gmail.com

#### Your own ideas

Propose your own ideas. Start points may be our QEP wikipage 
<https://github.com/Qucs/qucs/wiki/Qucs-Enhancement-Proposal> or Roadmap 
wikipage <https://github.com/Qucs/qucs/wiki/Roadmap>

**Expected results :** Something useful for Qucs

**Required skills :** C++, Qt, electronics or electrical engineering 

**Contact persons :** All Qucs developers



