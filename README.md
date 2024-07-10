# Report for Assignment 1 resit

## Project chosen

Name: Ismail Marghich

URL: https://github.com/IsmailMarghich/pendulum

Number of lines of code and the tool used to count it: 

I used lizard and there was a total of 20441 lines of code.

Programming language: Python

## Coverage measurement with existing tool

I used coverage.py to measure the branch coverage of the project, since the project used pytest I used these commands: 

coverage run --branch -m pytest

coverage report

Initial coverage results:

![Result](https://i.imgur.com/Tqc38fu.png)
![Result](https://i.imgur.com/pvoGiwP.png)
![Result](https://i.imgur.com/cUZswMK.png)
![Result](https://i.imgur.com/jI8ODVg.png)

# Coverage improvement

## Individual tests


### Function 1

Commit: https://github.com/IsmailMarghich/pendulum/commit/c3040be57a4017c596395710bd06fb0374f76780

Before charges:
![Result](https://i.imgur.com/uH98cyq.png)
After changes:
![Result](https://i.imgur.com/cMAgeEK.png)

The coverage has been improved by 2 percentage points, I have achieved this by adding another test case for the add_duration method, which allows you to add Duration objects together with the '+' operator. Specifically I added a test case where a run time error should be raised if you try add a date and a datetime object together as they are not compatible.


### Function 2

URL: https://github.com/IsmailMarghich/pendulum/commit/bb2bd87d3cde8e877267c66ee055fc3ef3083de6

Before changes:
![Result](https://i.imgur.com/s6T0ic6.png)
After changes:
![Result](https://i.imgur.com/eUazclM.png)

The coverage has been improved by 1 percentage points, I have achieved this by testing two string converstion methods which you can use on datetime objects. It seems this might have been forgotten by the developers, I made sure the methods return the correct output for a given input.

### Overall

Original coverage results:
![Result](https://i.imgur.com/Tqc38fu.png)
![Result](https://i.imgur.com/pvoGiwP.png)
![Result](https://i.imgur.com/cUZswMK.png)
![Result](https://i.imgur.com/jI8ODVg.png)

New coverage results:
![Result](https://i.imgur.com/xuiWINw.png)
![Result](https://i.imgur.com/VmyLfxF.png)
![Result](https://i.imgur.com/F3Udnnq.png)
![Result](https://i.imgur.com/njZ4EY7.png)

