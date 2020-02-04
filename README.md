# coding-challenge

landing pg

steps:

1. write down objective, identify mvp, timesinks, subtasks, etc
2. identify flaws and document why they are flaws and solutions
3. html skeleton
4. identifying critical css vs non-critical css
   4a) implement critical css inline
   grid layout
5. add form behavior and client-side form validation
6. implement non critical css, font-fallbacks, font-display
7. lighthouse, pagespeed insights etc to evaluate for accessibility & perf

design flaws:

- Header and footer menu styling inconsistent. Header menu has first letter capitalized, whereas bottom menu is all caps and heavier font-weight

  - ## Why is this a problem?
  - Solution:
    - Use header menu capitalization convention, with a bit heavier font-weight for stronger visual contrast with background

- 'Contacts' in header menu, 'Contact' in footer menu

  - Why is this a problem?
    - Repeated text with assumably same intent, but inconsistency results in differing meaning confusing user
  - Solution:
    - Eliminate Contacts

- 'Terms of Service' in form footnote, 'TERMS OF USE' in footer menu

  - Why is this a problem?
    - Repeated text with assumably same intent, but inconsistency results in differing meaning confusing user
  - Solution:
    - Eliminate TERMS OF USE, use Terms of Service as is convention

- Hero header has odd grammar

  - Why is this a problem?
    - Reflects poorly on legitamacy of brand and product
  - Solution:
    - Simple Way to Organize Your Inspirations -> A simple way to organize your inspirations

- Form footnote "By clicking 'Sign up' ..." is improperly placed.
  - Why is this a problem?
    - Positioning the TOS agreement within the form makes logistical sense, as the user would like to know what they are agreeing to prior to signing up. Furthermore, if the user is using a screenreader this is something that should be stated prior to signing up.
  - Solution:
    - Place in form to notify user what they are potentially agreeing to prior to signing up.

design opinion:

- Eliminate header and footer menu, move into hamburger menu
  - Why?
    - The primary objective of a landing page is having the highest conversion rate possible. Lots of text, options, anything that distracts the user from filling out the form / signing up / etc is detrimental to that objective
  - Solution
    - Hamburger menu will contain: About, Integrations, Pricing, Contact, Help, Privacy Policy
