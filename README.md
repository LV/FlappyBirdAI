# FlappyBirdAI
A neural network for Flappy Bird using reinforcement learning

This is my very first start at trying out any sort of machine learning or artificial intelligence. I am following Bluefever Software's tutorial which can be found [here](https://www.youtube.com/playlist?list=PLZ1QII7yudbebDQ1Kiqdh1LNz6PavzptO). His repo can be found [here](https://github.com/bluefeversoft/flappy_learning_pygame/).

## Start

### How to install and run

1. Clone this repository: `$ git clone https://github.com/LV/FlappyBirdAI` 
2. Go into the project directory and install the required packages: `$ pip3 install -r requirements.txt`
3. Run the program `$ python3 src/main.py`

### How to play

The premise of this game is to survive for as long as possible. Press **space** to jump. Press **esc** to quit the game.

### _master_ and _no-ai_ branches 

There are two branches of the repository, _master_ and _no-ai_. The _no-ai_ branch is version of the game you can play where as the _master_ branch will be where all the reinforcement learning will take place.

## The neural network

The neural network consists of two different inputs, five hidden layers, and one single output as demonstrated by the diagram below:

![neural network diagram](https://i.imgur.com/gBoEEi1.png "Neural Network Diagram")

#### Input nodes

- Input 1 (_i<sub>1</sub>_) will consist of the distance (in pixels) to the end of the nearest _upcoming_ pair of pipes.
- Input 2 (_i<sub>2</sub>_) will consist of the height between the bird and the middle of the _upcoming_ pipe pair gaps.

The inputs are demonstrated by the following photo:

![input demonstration](https://i.imgur.com/CGIYk63.png "Input demonstration")

The following diagram demonstrates how the neural network works (the actual program uses 5 hidden layers instead of 3):

![neural network diagram](https://i.imgur.com/BDmD0pa.png)
