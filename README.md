checkio-task-template
=====================

This is the basic CheckiO template for user generated tasks.
It has a fixed folder structure so please be careful with
your file and naming conventions.


## Tasks examples

[Triangle angles](https://github.com/Bryukh-Checkio-Tasks/checkio-task-triangle-angles)  

[Magic square](https://github.com/Bryukh-Checkio-Tasks/checkio-task-magic-square)


## Some more examples made by CheckIO's users

Several users took the challenge to create their own missions, you can view (and solve!) them on CheckiO.  
Like [Amachua](http://www.checkio.org/user/Amachua/)’s [Sudoku Solver](http://www.checkio.org/mission/sudokusolver/) or [Suwanditan](http://www.checkio.org/user/suwanditan/)’s [Periodic Table](http://www.checkio.org/mission/periodic-table/) (our CTO doesn’t even know how to solve this challenge!).


# Files definitions

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
The image files must be placed inside the `ìnfo/media` folder.
The link to these is defined as src="{{ MEDIA_URL }}/*image-name.png*"
Illustrations should be created with respect to our colors guide.
(`info/media/example.png` or  `info/vectors/color.pdf`)

##### Icons
Icons for the task are placed inside the `info/logo` folder.
Icons are created as a pair: **disabled.svg** for unsolved tasks and **enabled.svg** for solved tasks.
In the task runner you will see one of these where you can click on it.
Icons should be created with specified icons' colors from our colors guide: `info/media/color.pdf`.
Icons should be 128x128px and placed inside a grey colored block (size 116x116px) , outer corners rounded to a radius of 10px.
You can use the given templates.

#### story.html
This is a funny story about the task, it does not need to
explain the task's goal. A paragraph of div with the story
class does not show in the editor's task description.

#### short_task_description.html
A summary of the task.


# A brief description of the other folders:

### editor folder

##### options.json
It's **not necessary** to change it.
Further description of this will be added later.
##### templates.html
This file describes layout and structure for the tests explanation or “try it”.     
It's **not necessary** to change it.
Further description of this will be added later.

#### editor/animation Folder

##### init.js
This file describes an animation for the tests explanation or “try it”.       
At `python: 'function name'` and `js: 'function name'` you can state the identifier your function is to be called with (line 11, 12). 
It's **not necessary** to change it.
Further description of this will be added later.

##### init.css
This file describes styles for the tests explanation or “try it”.       
It's **not necessary** to change it.
Further description of this will be added later.

#### editor/initial_code Folder

##### js-node
##### python_3
These 2 files hold the code which users will see as a starting template for the node.js  and the python3 interpretor.
If you use strings for python3 you can use unicode strings.

### hints Folder

##### _slug.html
You have the option to give some hints here.
It’s **not necessary** to change it.
Further description of this will be added later.

### verification Folder
The files in this folder are for 'Check'.
They contain a referee and additional files with your tests.

##### referee. py
At `python: 'function name'` and `js: 'function name'` you can state the identifier your function is to be called with (line 41, 42).
This file also contains a referee and additional files for tests; in the file itself you find a detailed description for its use.
##### tests. py
Here you can add your test cases; in the file itself you find a detailed description for its use.
Also, an example is included.


