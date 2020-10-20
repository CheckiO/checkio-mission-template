CheckiO Mission
=====================

This is a mission repository for projects like [JS.CheckiO](https://js.checkio.org/), [PY.CheckiO](https://py.checkio.org), [Empire of Code](https://empireofcode.com)

In order to check this mission you can either find it on one of the listed projects or use [checkio-client](https://github.com/CheckiO/checkio-client)


# Files definitions

Below you can read an explanation for the role of each folder and file inside the project.   

### Info folder

This folder contains information about the task's mission.   

#### task_description.html

This file is a description for your task. Here, you should explain the goal of the task.   
When writing this file, you must use proper HTML syntax for the description to be readable on the site as it will be inserted on the task page as a HTML block.    
If you are not familiar with html code, you can find a choise of on-line free html editors on the www .  

##### Task's text
Here is where you place the main description of the task.    
You can insert some images for explanation (see below for information about images)    
and you can use html tags as ```em```, ```strong``` or ```pre``` to display formulas or example code.   
Each paragraph or div element can have the class  "for_editor_only" or "for_info_only".   

**"for\_editor\_only"** – means that the element will only show in the editor mode.   

**"for\_info\_only"** – will only show up in the main task description.   

##### Input and Output
This is a short description of the input and output data.

##### Example
This section gives some examples for the task.   
You can use the ```pre``` tag with class "brush: python" for syntax highlighting.   

##### Images
You can paste some images in your text to illustate your task.   
The image files must be placed inside the `ìnfo/media` folder.   
The link to these is defined as src="{{ MEDIA_URL }}/*image-name.png*"   
Illustrations should be created with respect to our colors guide: `info/colors.pdf`.   
     
##### Example     
```
<p class="for_info_only" style="text-align: center;">
    <img  title="image-name" src="{{MEDIA}}image-name.png" alt="image-name" style="max-height: 100px"/>
</p>
```   
This will place a picture which will scaled down to a height of 100 pixels in a html paragarph.   
Due `class="for_info_only"` it will only show up in the main task discription,   
where it will be alined to the horizontal center of the page `style="text-align: center;`.   

##### Icons
Icons for the task are placed inside the `info/logo` folder.   
Icons are created as a pair: **disabled.svg** for unsolved tasks and **enabled.svg** for solved tasks.   
The task runner will show either one of these icons and users will be able to click on it.   

##### Icon specifications
All icons shoud match the folowing specifications:    
**Colors:** Icons should be created with the specified icons' colors from our colors guide: `info/media/color.pdf`.       
**Size:** Icons should be sized 128x128 px and placed inside a dark grey(#737370) colored block (size 116x116 px), outer corners rounded to a radius of 10px.    
**Icon status:** On both icons,  'disabled' and  'enabled', shows the same drawing represented in light grey(#EBEDED).   
At the 'enabled' icon however, some details of this drawing have been accentuated by a blue(#82D1F5) collor to highlight its active status.    
   
You can use the given templates.    

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
If you use a string for python3 -- use an unicode string.

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
This file also contains a referee and additional files for tests.   
`python: 'function name'` and line 42: `js: 'function name'`.  At `'function name'` you can state the identifier of your function to which the arguments you listed at **test.py** will be parsed for testing.   
In the file itself you find a detailed description for its use.

##### tests. py
This file holds a dict with all you tests; its keys represent the categorie names of your tests eg. basics, extra, etc.      
In the categories each test is dict again with 3 keys, ie.       
`"input"` -- an arguments list as for your functions input,   
`"answer"` -- the correct data to be retuned for the arguments from the input list,   
`"explanation"` -- this a not necessary key, it's used to provide additional animation data, its value shall be `None` (or just remove this key) if you don't want use an animaion.     
in the file you will find a detailed description, an example is also included.



