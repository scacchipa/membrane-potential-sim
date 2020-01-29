# membrane-potential-sim
Simulates membrane potential and the action potentail of exitables cells.

It is written on processing, an open-source graphical library and uses the Java language, with additional simplifications. It is meant to be a flexible software sketchbook. I choose to processing since trying ideas and sharing them easy and straight forward. 

The program works by simulating an excitable "cell" as a class, there are three main methods "membrane potential", "depolarized" and "conduct". Membrane potential method uses a simplified version of the  Goldman-Hodgkin-Katz (GHK) voltage equation. ![Medical physiology Walter Boron](https://i.imgur.com/54bCzEh.png)
The alfa variable in the equation is the quotient of the permeabilities between Na and K (PNa/Pk). The number is very low during resting potential since the permeability of K predominates. During an action potential these changes, the permeability of Na increases rapidly in a sigmoid fashion. The depolarize method generates this same change in the alfa variable producing an asudden increase in membrane voltage. 

The first action potential is trigger through an automatic cell with a timmer, it then propagates thanks to the conduct method.

### Run

1- Install > processing https://processing.org/download/

2- Clone repository

3- Run main.pde insde the main folder

### Demo
##### Single cell Vm 
![](https://media.giphy.com/media/IeGEyz3wNrq2pzlvIj/giphy.gif)

#### Array of cells
First square from the right triggers the rest in a secuential fashion.
When white the cell is in resting potential, when red it has been depolarized. 

![](https://media.giphy.com/media/QZ1anIbB4oDKCK22bG/giphy.gif)
