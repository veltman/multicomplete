# Multicomplete
### *Autocomplete with a variable number of selections displayed inline*

This is a demo of how to replicate the tag autocomplete functionality of sites like Stack Overflow that allow you to enter any number of tags in the same field with the autocomplete following along.

This particular demo uses ([http://jqueryui.com/demos/autocomplete/](jQuery UI Autocomplete) but the basic concept can easily be applied to any autocomplete widget.

Each multicomplete consists of a `<ul>` styled to look like a text input.  Inside that `<ul>` is a `<li>` with an unstyled `<input>` in it.  That input receives user input and functions like a normal autocomplete.  When the user chooses something from the autocomplete, it creates a new `<li>` immediately before the text input and clears the text input of its contents. That new `<li>` includes the selection label, a hidden input with its value, and an 'X' link to remove the tag.  This example also incorporates dupe-checking, skipping tags that have already been selected.  You can also add support for negative operators for something like a search field by simply adding a different class to the new `<li>` and modifying its value if the input begins with '-' or the word 'not'.

### Contact  
[noah@noahveltman.com](mailto:noah@noahveltman.com)  
[http://noahveltman.com/](http://noahveltman.com/)