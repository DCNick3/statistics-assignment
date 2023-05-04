
The first task included a lot of computations & equation solving, so I decided to use Mathematica language to do it. It's a functional language with focus on symbolic computation, which is useful for solving equations.

Then it somehow snowballed into implementing the second task in Mathematica too.

The repository (https://github.com/DCNick3/statistics-assignment) contains `task*.nb`, which are the Mathematica notebooks I used to solve the tasks. They are also rendered as PDF files so that one could look at the code without having Mathematica installed.

## Task 1: Bayesian Statistics

The [notebook](task1.pdf) contains all relevant info

## Task 2: Simulated Annealing


I've tried doing the annealing with three temperature decay coefficients: `0.9`, `0.95` and `0.99`

The lengths of the resulting paths were as follows:

|coefficient|distance, km|
|---|--------------------|
|0.9|40 213.4|
|0.95|42 154.4|
|0.99|25 085.6|

Here's also the plot of distances over time:

![over_time](https://user-images.githubusercontent.com/10363282/236345360-a672e976-ac2b-465c-a560-d13a2afabfab.png)

The `0.95` (called middle) seemed to have some trouble settling at the beginning, probably due to bad luck, and came to worse solution.

For visualization I used built-in mathematica GIS support, so it already came with a reasonable projection and graph visualization capabilities.

Here's a visualization for temperature decay coefficient `0.99`.

[animation.webm](https://user-images.githubusercontent.com/10363282/236343608-6e1d03f7-1c94-41c3-9493-13923e87de63.webm)

Looking at the final solution that was found with the `0.99` decay coefficient seems pretty reasonable to me.

