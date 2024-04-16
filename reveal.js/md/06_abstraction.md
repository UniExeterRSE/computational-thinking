# Abstraction

Abstraction is about simplifying problems, making them easier to solve. The idea is to identify and then ignore information that is not essential.

## Relation to programming

Abstraction is an approach that helps solve problems. A core component of programming is about creating and composing abstractions, using objects and functions to represent and define the solution. 

Abstraction works by establishing a level of complexity at which a person interacts with a system, suppressing the more complex details below the current level. Abstraction allows programmers to define objects and functions that can interact with each other in a predictable way without having to understand the underlying details of their implementation. 

When you see a simple interface covering a more complex implementation, this is abstraction. 


## Example - the London tube map

The problem the tube map is designed to solve is to help people navigate the underground system in London. The essential information to complete this task is:

1. the name of each station
2. which lines each station is on
3. the order of the stations on each line
4. which stations are intersections between lines
5. which stations have onward connections to other transport modes (e.g. National Rail)
6. which stations have step free access


<img src="fig/tube-geography.jpg" height=500>

Information that is not essential to this problem is the precise location of each station. So it is removed...


<img src="fig/tube-map.jpg" height=600>


When on a particular line, even less information is required...

<img src="fig/hammersmith-line-2024.png" height=400>


## Example - motor car

The interface of a car is simple

* steering wheel
* accelerator
* brake
* gear stick

However, these cover a much more complex machine. You learn that pressing the accelerator makes the car go faster but you are not taught how the acceleration actually works - because the details of this are not important for you to drive the car.


### Activity: Tour Guide

<div class="container">
<div class="reveal col">

You are a hotel tour guide. Tourists staying in your hotel expect to be taken on a tour visiting all the city’s attractions. Using this map showing locations of all the attractions, and how to get from one to another, you must work out a route that starts from the hotel and takes your tour group to every tourist site. 

* Tourists will be unhappy if they pass through the same place twice
* They must end up back at their hotel that evening

How would you solve this? What is the minimal amount of information you need to extract from the map to solve it?
</div>
<div class="col">
<img alt="tour guide" src="../images/tour_guide.png" height="400">
</div>
</div>


### Activity: Knight's Tour

<div class="container">
<div class="reveal col">

On the cross shaped board below, a chess Knight can move two spaces in one direction and then move one square at right angles, or vice versa, as it moves in a chess game. It jumps to the new square without visiting any in between, and must always land on a square on the board. Find a sequence of moves that starts from Square 1, visits every square exactly once and finishes where it started.
</div>
<div class="col">
<img alt="knightstour" src="../images/knights_tour.png" height="400">
</div>
</div>


### Are these problems similar? 

How might you represent the Knight's Tour in a different way to simplify finding a solution?

Abstraction can be incredibly powerful. In the face of a complex problem,  the ability to separate what aspects of a problem are important for solving it, and what are spurious details really helps to design a computational solution.

Abstraction not only makes a problem easier to solve, it should also lead to a more efficient solution as you are not spending time processing information that does not help you get to the solution.