Password Strength Checker
=========================

A Javascript based tool that checks and reports password strength instantly.  An attempt to work
with mustache (http://mustache.github.com/). 

### REQUIREMENT
Needs jQuery and Mustache.

### VERSION
alpha

### DEFINITION
Password Strength is probably defined by both character space and length.  
alpha space is 52 [a-zA-Z]
alphanumeric space is 62 [0-9a-zA-Z]
with 30 symbols on top of alphanumeric, 92 space
Note that 52^8 > 92^6.  This means 8 alphabete characters is harder to break than 6 characters of jiberish.  This means that having password that is hard to remember does not neccessarily means they are stronger.  

### SCORE SYSTEM


### CONTRIBUTOR
Harris Wong [harriswong](https://github.com/harriswong)

### TESTING
TODO

---
More information can be found at: https://github.com/harriswong/pwd_str