# Number-Guessing-Game
[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/guess-number-bo/)

A simple PyPi package for guessing a number. Players take turns to guess a number within a certain range. The program will respond if the number is too large or small. The player who got the number first wins. 

## Installation

``` 
pip install guess_number_bo
```

## How to play?

```
>>> from guess_number_bo import GuessNumber
>>> gn = GuessNumber()                     
>>> gn.play()
Welcome to guessing number game!
The default game is for 2 players. Do you want to customize your game? [N/y]

```

## How to publish to PyPi?

```
python setup.py sdist
pip install twine

# commands to upload to the pypi test repository
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
pip install --index-url https://test.pypi.org/simple/ dsnd-probability

# command to upload to the pypi repository
twine upload dist/*
pip install dsnd-probability
```