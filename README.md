# Report for Assignment 1 resit

## Project chosen

Name: Ismail Marghich

URL: https://github.com/IsmailMarghich/pendulum

Number of lines of code and the tool used to count it: 

I used lizard and there was a total of 20441 lines of code.

Programming language: Python

## Coverage measurement with existing tool

<Inform the name of the existing tool that was executed and how it was executed>
I used coverage.py to measure the branch coverage of the project, since the project used pytest I used these commands: 

coverage run --branch -m pytest

coverage report

<Show the coverage results provided by the existing tool with a screenshot>

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

<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced tests for function 1>

<Provide a screenshot of the old coverage results for such function>

<Provide a screenshot of the new coverage results for such function>

<State the coverage improvement with a number and elaborate on why the coverage is improved>

### Overall

<Provide a screenshot of the old coverage results by running an existing tool (the same as you already showed at the beginning of the report)>

<Provide a screenshot of the new coverage results by running the existing tool using all test modifications>
