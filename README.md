# Python developer test task (GIS)
![python3](https://img.shields.io/badge/-python3-yellowgreen)
![docker](https://img.shields.io/badge/-Docker-orange)
![GIS](https://img.shields.io/badge/-GIS-blue)

## Task
You have to develop a streets colouring algorithm using python3 and create a really simple web server where user can attach a file which should be processed. Your algorithm should paint lines in the same colour when you think it is a single street.
1. You don't have to match coordinates with streets from real world. Those streets were taken just for example.
2. Don't use any 3-rd party services, you don't need them.
3. Create a solution just based on the information in the file.
4. It's an just an algorithimic task.

## Requirements:
- Server has to return generated image in base64 
- Solution has to generate images large enough to distinguish lines 
- Your repo with solution should contain file with explanation of how your algorithm works (it can be added to README.md with section Explanation)
- Web site should allow to generate .png from sample data. In other words sample data should be embedded into the solution (create separate button for that)
- Solution has to be dockerized
- Solution should work just by running './run.sh'

## Hints
- For plotting purpose you can use 'matplotlib'

## What will be checked during test task evaluation?
- It can be run using './run.sh' on Linux with docker
- Efficiency of solution
- Solution should correspond to requirements
- Understanding and usage of [SOLID](https://en.wikipedia.org/wiki/SOLID)
- Understanding and usage of [OOP](https://en.wikipedia.org/wiki/Object-oriented_programming) or FP
- [Code style consistency](https://blog.devgenius.io/why-code-consistency-is-important-9d95bdebcef4)
- Code readability and [cognitive complexity](https://docs.codeclimate.com/docs/cognitive-complexity#:~:text=Cognitive%20Complexity%20is%20a%20measure,be%20to%20read%20and%20understand.)
- Clean git history with understandable commit messages

## Examples
Sample input (but multilines are splitted into simple lines).
![Initial data](https://raw.githubusercontent.com/zakhar-bozhok-jito/jun-python-gis-test-task/master/out-examples/initial.png)
Possible generated output of the solution. Lines are randomly colourized. But some of different lines were occasionaly colourized the same color.
![Sample output1](https://raw.githubusercontent.com/zakhar-bozhok-jito/jun-python-gis-test-task/master/out-examples/processed-solid.png)
Possible generated output, but lines have also different line styles.
![Sample output2](https://raw.githubusercontent.com/zakhar-bozhok-jito/jun-python-gis-test-task/master/out-examples/processed.png)
