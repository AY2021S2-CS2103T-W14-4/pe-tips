# pe-tips

# Problematic Inputs

## Long Inputs
Long inputs can cause potentially unhandled errors such as
- UI not displaying whole text
- UI layout getting disrupted

Fields such as name, description, email, tags, and other free text inputs are susceptible.

Examples:  
`Superlonginputtestcasemaycausesomeerrorswhichmaynothavebeenhandled`
`longemail@superlonginputtestcasemaycausesomeerrorswhichmaynothavebeenhandled.com`


## Duplicate Inputs
Duplicate inputs may/may not be allowed depennding on the UG. Check if behaviour is as mentioned and see if any bugs are found when duplucate instances are allowed.
- Duplicate Instances, tags, etc.

Examples:  
`t/manytag1 t/manytag1 t/manytag1 t/manytag1`
