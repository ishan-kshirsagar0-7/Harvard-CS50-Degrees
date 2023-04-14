# Harvard CS50 AI (Week 0) Project 1 : Degrees

This is the first project of [Harvard CS50's Introduction to Artificial Intelligence course](https://cs50.harvard.edu/ai/2020/), Week 0.

## My Outputs

![Screenshot of my output on terminal](https://cdn.discordapp.com/attachments/1091358303063396496/1096391694452281344/degrees.jpg)

## Objective

Write a program that determines how many “degrees of separation” apart two actors are.

## Background

According to the [Six Degrees of Kevin Bacon game](https://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon), anyone in the Hollywood film industry can be connected to Kevin Bacon within six steps, where each step consists of finding a film that two actors both starred in.

In this problem, we’re interested in finding the shortest path between any two actors by choosing a sequence of movies that connects them. For example, the shortest path between Jennifer Lawrence and Tom Hanks is 2: Jennifer Lawrence is connected to Kevin Bacon by both starring in “X-Men: First Class,” and Kevin Bacon is connected to Tom Hanks by both starring in “Apollo 13.”

We can frame this as a search problem: our states are people. Our actions are movies, which take us from one actor to another (it’s true that a movie could take us to multiple different actors, but that’s okay for this problem). Our initial state and goal state are defined by the two people we’re trying to connect. By using breadth-first search, we can find the shortest path from one actor to another.
