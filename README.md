checkio-task-template
=====================

Base CheckiO template for users task.
It have fixed folder's structure, please be careful with it and files' names.

Tasks examples
--------------
https://github.com/Bryukh/checkio-task-transposed-matrix

Files definition
----------------

Below you can read explanation for role of each file of folder inside.

description.html
----------------

It's description for you task. Here you should explain the goal of the task.
For this using HTML syntax. This block will be inserted at the task page.

#### Story
First paragraph has class "story" -- this is some funny story about task, it does not explain task's goal.
This is not necessary. This is paragraph does not show in the editor's task description.

#### Task's text
Next, the main description of the task. You can insert some images 
for explanation (see bellow about images). Also you can use html tags as *em* **strong** or *pre* for some formulas.
Each paragraph or *div* element can have class "for_editor_only" or "for_info_only".
"for_editor_only" -- it's showed only in the editor mode.
"for_info_only" -- it's showed only main task's description.

#### Input and Output
This is short description of input and output data.

#### Example
This is some examples for your task. You can use for this *pre* tag with class "brush: python" for syntax highlight.

#### Images
You can paste your images inside task. The files for these must be placed inside **illustrations** folder.
The link defined as src="/static/files/illustrations/*image-name.png*"
Illustrations should be created with specified colors from colors guide (*color.pdf*)

#### Icons
Icons for task placed inside *icon* folder. Icons created as pair:
*disabled.png* -- for unsolved tasks.
*enabled.png* -- for solved tasks.
In the task runner you can see the both icons with click to it.
Icons should be created with specified icons' colors from colors guide (*color.pdf*).
Icons must have size 128x128 and placed inside grey color with size 116x116 at center with border radius 10.
Just use given template.

task.json
---------
It's task's config with some useful info.

**task_name** -- The name of the task.

animation_cfg.json
--------
This file describe sizes of animation and tryit panels.

**tryit\_results\_height** -- the height of tryit results. If you dont want to use tryit, then set it to 1.

**tryit\_results\_width**  -- the width of tryit results. If you dont want to use tryit, then set it to 1.

**animation\_panel\_width**  -- the width of animation's panel.

**console\_height** -- the height of bottom console. As usual, set it as tryit\_results\_height + 30


start_code.py
-------------

The code which user will see as a start template.


animation.js
------------

This file describe an animation for tests explanation or tryit.
It's **not necessary** to change it.

Description of this will be later.

animation.js
------------

This file describe styles for tests explanation or tryit.
It's **not necessary** to change it.

Description of this will be later.

template.html
-------------

This file describe layout and structure for tests explanation or tryit.
It's **not necessary** to change it.

Description of this will be later.

