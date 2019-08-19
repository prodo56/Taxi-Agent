# Taxi Agent

### Table of Contents

1. [Project Motivation](#motivation)
2. [Agent Environment](#environment)
3. [Project Components](#projectComponents)
4. [Instructions](#instructions)
5. [Results]("results")
6. [Licensing, Authors, and Acknowledgements](#licensing)


### Project Motivation <a name="motivation"></a>
In this project, I have used OpenAI Gym's Taxi-v2 environment to teach a taxi agent to navigate a small gridworld using Q-Learning. The goal is to adapt all that you've learned in the previous lessons to solve a new environment!.

### Agent Environment <a name="environment"></a>

```
+---------+
|R: | : :G|
| : : : : |
| : : : : |
| | : | : |
|Y| : |B: |
+---------+
```

* There are four designated locations in the grid world indicated by R(ed), B(lue), G(reen), and Y(ellow). When the episode starts, the taxi starts off at a random square and the passenger is at a random location. The taxi drive to the passenger's location, pick up the passenger, drive to the passenger's destination (another one of the four specified locations), and then drop off the passenger. Once the passenger is dropped off, the episode ends.

* There are 500 possible states, corresponding to 25 possible grid locations, 5 locations for the passenger, and 4 destinations.
* There are 6 possible actions, corresponding to moving North, East, South, or West, picking up the passenger, and dropping off the passenger.


### Project Components <a name="projectComponents"></a>
There are two components in this project.

1. Agent

	- `agent.py`

		- class to store Q-Table values with functions to update Q-Table and select next action

2. Monitor
	
	- `monitor.py`

		- interact function tests how well your agent learns from interaction with the environment.


### Instructions <a name="instructions"></a>

Run `main.py`.


### Results <a name="results"></a>

```
Episode 20000/20000 || Best average reward 9.2246
```


### Licensing, Authors, and Acknowledgements <a name="licensing"></a>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

* [Udacity](https://www.udacity.com/)
