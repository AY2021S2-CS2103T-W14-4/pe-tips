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


## Modifying an object where there is another object that is a duplicate or has identical fields
Modifying the 1st object may/may not modify its duplicate or other objects similar to the 1st object


## Deleting a specified object when there is another duplicate object
Deleting a specified object may/may not delete duplicate objects which arent specified.


## Duplicate items might have an additional identifier added to distinguish between duplicates
For example, if the app allows adding two duplicate objects with the same name, the name/id of one of the duplicates might have a counter attached to it. In this case, this might cause issues when editing/deleting these objects


## Date Inputs
- Check if leap years and invalid dates are handled properly.
- For certain products, entering past dates may not make sense to the functionality
- Check of past dates cause errors

Invalid Dates:  
`2021-02-29, 2021-02-30, 2021-11-31, 2021-11-32`

Past Dates:  
`1999-02-27, 0000-02-09`

Similar principles can be applied to time.

## DG Possible Bugs:
- Broken Links (DevOPS code coverage link, Setting up user Guide)
- UML Diagram Errors (Missing Labels/arrows, wrong arrow directions, incomplete diagrams)
- NFR have errors
- Grammatical/Spelling Errors





