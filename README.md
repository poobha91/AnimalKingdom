# AnimalKingdom
Animal Kingdom – The Critter program
Abstract
In this Animal Kingdom program will not be writing a main method; instead, will be defining a series of objects that become part of a larger system. The only way a critter can move is to wait for the simulator to ask it for a move. The simulator is in control, not the critters class. Critters move around in a world of finite size that is enclosed on all four sides by walls. I should include a constructor for each class I write as most classes need to keep track of number of moves or other variables. For classes that always use the same Strings/Colours, should declare them as class constants. The simulator has several supporting classes that are included Critter, CritterMain, CritterModel, CritterFrame, CritterInfo (interface), CritterPanel, FlyTrap, and Food these classes can ignore in general. When compile CritterMain, these other classes will be compiled. Only classes will have to modify and recompile are CritterMain to add the frame of animals and own individual 5 Critter classes and its behaviour of that classes.

Introduction
Java is a popular high-level programming language developed by Sun Microsystems (now Oracle) in the mid-1990s. Java was designed to be platform-independent, meaning it can run on any platform or operating system that has a Java Virtual Machine (JVM) installed. Java is widely used for developing various types of applications, including web applications, desktop applications, mobile apps, and games.

IntelliJ IDEA is a popular Integrated Development Environment (IDE) for Java development. It is developed by JetBrains and is widely used by Java developers worldwide. IntelliJ IDEA provides a wide range of features, including code analysis, code completion, debugging, and version control integration. IntelliJ IDEA is available in both free and paid versions, with the paid version providing more advanced features and capabilities. IntelliJ IDEA also supports many other programming languages, including Kotlin, Python, and JavaScript.

The Animal Kingdom project is a simulation game in which different types of animals are represented as objects and interact with each other in a virtual world. The objective of the project is to design and implement a Java program that simulates the behaviour of the animals and allows users to interact with them in different ways.

The Animal Kingdom project involves creating a superclass called "Critter" that defines the basic behaviour of all the animals in the simulation. Then, required to create five subclasses of "Critter," each representing a different type of animal: Bear, Tiger, White Tiger, Giant, and Ninja Cat. Each subclass has its own specific behaviour and characteristics.

The project also requires implementing a graphical user interface (GUI) for the simulation, allowing users to view the animals and interact with them using mouse clicks and keyboard events. The GUI should display the current state of the simulation and allow users to control the simulation speed and other parameters.

Overall, the Animal Kingdom project is a fun and engaging way to apply object-oriented programming principles in a real-world simulation. By completing this project, can gain valuable experience in developing Java programs using object-oriented design and learn how to build interactive user interfaces in Java.

Gameplay

This simulator provides great visual feedback about where critters are, so can watch them move around the world, to see the what direction critters are facing this simulator has a debug button to show the direction. When click to debug button critters will be displayed as arrow characters that indicate the direction they are facing. The simulator also indicates the "step" number as the simulation proceeds by default start from 0 (zero). 

Let’s say we set all animals have just 30 bears, tigers, white tigers, giants, and ninja cats. This numbers can set in CritterMain class. First, we see about the Bears behaviours; should see about half of them being white and half being black. Initially they should all be displayed with slash characters. When you click “step” button, they will all switch to backslash characters. When you click “step” button again they will go back to slash characters and so on. When you click “start” button, you observe the bears heading towards walls and then hugging the walls in a counter-clockwise direction. They will sometimes see into each other and go off in other directions, but their tendency should be to follow along the walls. 

Next look into tigers should see about one third of them being red and one third being green and one third being blue randomly. When click to “step” button the colours will change on every 3rd steps. They will keep these initial colours for every 3 moves. That means that they will stay same colour while the simulator is indicating that it is step 0, step 1, and step 2. They should switch the colours when the simulator indicates that are up to step 3 and will stay with these new colours for steps 4 and 5. Then you will see a new colour scheme for steps 6, 7, and 8 and so on. When click “start” button you will see them bouncing off walls. When they bump into a wall, they will turn around and head back in the direction they came. This white tiger should behave just like a tiger except that they will be White. They will also be lower-case until they infect another Critter, then they "grow up”.

Lets look into giant now, while running the simulator at first all will be displayed as “fee”. This will remain until steps 0 to 5th and then when get to step 6th they will all switch to displaying as “fie” and will stay for the next 6 steps. After that following steps after “fie” will change to “foe” and will remain for the next 6 steps; and then will change to “fum” on next 6 steps. After “fum” it will goes back to “fee”. When click to “start” button can see the same kind of wall-hugging behaviour that bears have, but this time in a clockwise direction.
Figure in above show how the animals moving when click to “start” button. The numbers on right side show the steps counts and number of infected animals (decreasing) and infect the enemy (increasing). 

 

In this figure shows when click to “debug” button; the animals show as the arrow and then the direction they are facing. At here the “step” and “next 100” button will be helpful to see the animal movements. “step” button for 1 step at a time and “next 100” will jump 100 steps on one click. 

You may can click “stop” button to pause the simulation and at slow and fast slider can adjust the speed of the animals. 

 
After a long run you can who will still stand until the end. When animal equal to zero it means those animals all are infected. 
