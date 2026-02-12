# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

Summarize your learnings from the lab here.
We learned about implementing a naive equation, SOP equation, and POS equation in Verilog. Additionally, we learned how to load them onto a board. 
We learned more about creating and simplifying KMaps and checking the correctness of our Verilog files via the simulation.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
In a KMap, the actual shape is a torus - the edges are connected. The 2d grid is simply a representation of that shape.

### Why are the names Sum of Products and Products of Sums?
A Sum of Products expression is comprised of ORed AND statements - it is the sum (OR) of a group of products (AND).
A Product of Sums expression is comprised of ANDed OR statements - it is product (AND) of a group of sums (OR).

### Open the test.v file – how are we able to check that the signals match using XOR?
In test.v, there are two conditional statements - one that compares the outputs of naive with minterm, and one that compares the outputs of naive with maxterm.
The conditional checks to make sure that the outputs match - it will only execute if they differ (and output a corresponding error message). 
