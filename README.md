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
Note that 52^8 > 92^6.  This means 8 alphabet characters is harder to break than 6 characters of jiberish.  This means that having password that is hard to remember does not neccessarily means they are stronger. We can also change the above example to the following equation:
x^y = (x+40)+^(y+b), when x is the alphabet set, and x+40 is the alphanumeric+symbol set.  We need to solve for 'b'.
Apply constraints based on normal use case, set x = 52, numbers of alphabets, we get
52^y = 92^(y+b)
b ~= 1.2y

so if we have 6 characters of alphanumberic+symbol, it is almost as strong as 8(round(6*1.2)) characters of alphabet set.  ie. "asd$%1" is as strong as "helloyou".

### SCORE SYSTEM
- length of 8 get 1 point
- length of 10+ gets 1 point
- having 1 non alphabet character gets 1 point
- having 2+ non alphabet character gets 1 point

### CONTRIBUTOR
Harris Wong [harriswong](https://github.com/harriswong)

### TESTING
TODO

---
More information can be found at: https://github.com/harriswong/pwd_str
