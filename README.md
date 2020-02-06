# coding-challenge

landing pg

#### steps:

1. write down objective, identify mvp, timesinks, subtasks, etc
2. identify flaws and document why they are flaws and solutions
3. html skeleton
4. identifying critical css vs non-critical css
   4a) implement critical css inline
   grid layout
5. add form behavior and client-side form validation
6. implement non critical css, font-fallbacks, font-display
7. lighthouse, pagespeed insights etc to evaluate for accessibility & perf

# design considerations and revisions:

## Inconsistent grammar and term usage
##### EX1: Header and footer menu styling inconsistent. Header menu has first letter capitalized, whereas bottom menu is all caps and heavier font-weight
##### EX2: Contacts' in header menu, 'Contact' in footer menu
##### EX3: 'Terms of Service' in form footnote, 'TERMS OF USE' in footer menu
### Why is this a problem?
* Repeated text with assumably same intent, but inconsistency results in differing meaning confusing user
### Solution
* Why is this a problem?
   * Solution:
      * Eliminate duplicate fields, converge on single capitalization convention (first letter capitalized only)
    
## Usage of ```.ttf``` fonts
### Why is this a problem?
* ```.ttf``` fonts are 50%+ heavier than woff(2) format. woff(2) is a format compressed out of the box
### Solution
* Replace provided ```.ttf``` fonts with ```.woff2```
