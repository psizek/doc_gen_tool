# doc_gen_tool
This is a tool for generating documents programatically (e.g. from a database).  This has two main components:

## forget.py
This script populates tags inside of strings according to a tag dictionary, where tags are in the form [[tag##default]], and the dictionary is in the form {tag : value}. If the dictionary does not contain a tag, the default value is used instead. You can think of this as a "filling out a form" tool. The forms/ directory is where we look for forms saved in a file.

## tagg.py
This script runs python code inside of tags in a string. Tags are in the form {{code_to_run}}. Functions to be used with this must be listed in funcs.py

##The example
I've added main.py along with a file in forms and output as an example.

##Other notes
Maybe in the future I'll do something more with this (don't fix the hardcode the forms and output paths and make it a command line tool), but I'm satisfied for now with where it is.
