checkio-task-template
=====================

This is the basic CheckiO template for user generated tasks.
It has a fixed folder structure so please be careful with
your file and naming conventions.


## Tasks examples

[Traingle angles](https://github.com/Bryukh-Checkio-Tasks/checkio-task-triangle-angles)  

[Magic square](https://github.com/Bryukh-Checkio-Tasks/checkio-task-magic-square)


## Some examples

Several users created their own missions, and you can view (and solve!) them on CheckiO.  
Like [Amachua](http://www.checkio.org/user/Amachua/)’s [Sudoku Solver](http://www.checkio.org/mission/sudokusolver/). Or [Suwanditan](http://www.checkio.org/user/suwanditan/)’s [Periodic Table](http://www.checkio.org/mission/periodic-table/) (our CTO doesn’t even know how to solve this challenge!).


# Files definition

Below you can read an explanation for the role of each folder and file inside the project.

### Info folder

This folder contains information about the task's mission.

#### task_description.html

This file is a description for your task.
Here, you should explain the goal of the task.
When writing this file, you must use proper HTML syntax for the description to
be readable on the site as it will be inserted on the task page as a block.

##### Task's text
Next, you must write the main description of the task.
You can insert some images for explanation (see below for
information about images) and you can use html tags as 
```em```, ```strong``` or ```pre``` to display formulas or example code.
Each paragraph or div element can have the class
"for_editor_only" or "for_info_only".

**"for\_editor\_only"** – means that the element will only show in the editor mode.

**"for\_info\_only"** – will only show up in the main task description.

##### Input and Output
This is a short description of the input and output data.

##### Example
This section gives some examples for the task.
You can use the ```pre``` tag with class "brush: python" for syntax highlighting.

##### Images
You can paste your images inside the task.
The image files must be placed inside the illustrations folder.
The link is defined as src="{{ MEDIA_URL }}/*image-name.png*"
Illustrations should be created with specified colors from our colors guide. (*color.pdf* or *example.png*))

##### Icons
Icons for the task are placed inside the logo folder.
Icons are created as a pair: 
**disabled.svg** for unsolved tasks and **enabled.svg** for solved tasks.
In the task runner you can see both icons with click to it.
Icons should be created with specified icons' colors from our colors
guide (*color.pdf*).
Icons should be 128x128px and placed inside a grey color block (size 116x116px) with a border radius of 10px.
Use the given template.

#### story.html
This is a funny story about the task, it does not need to
explain the task's goal. A paragraph of div with the story
class does not show in the editor's task description.

#### short_task_description.html
A summary of the task.

### Verification Folder

This folder contains a referee and additional files with tests, if you need these. Also it contains the folder with initial code.

#### initial_code/interpretator

Here is the code which users will see as a starting template for the interpretator.

If you use a string for python2.7 -- use an unicode string.

### Editor folder


#### templates.html

This file describes layout and structure for the tests explanation or tryit.
It's **not necessary** to change it.

Further description of this will be added later.


#### Animation Folder

#### init.js

This file describes an animation for the tests explanation or tryit.
It's **not necessary** to change it.

Further description of this will be added later.

#### init.css

This file describes styles for the tests explanation or tryit.
It's **not necessary** to change it.

Further description of this will be added later.


