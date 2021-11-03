# EducationPlatformLayout

## What did I learn from this project?
- CSS Grid might behave a little weird when they're nested some levels deep, as mentioned [here](https://github.com/w3c/csswg-drafts/issues/1777), the meaning of `1fr` when defining the proportions of the grid items implicitly means `minmax(auto, 1fr)` which leads to situations where some heights are not defined and grid items end up overflowing their grid containers. The quick solution is to use `minmax(0, 1fr)` instead of `1fr` (or whatever needed number of course).
- This project wasn't meant to be responsive, however I tried to do so after finishing the overall layout and it was more complicated than I thought it'd be, so maybe that's why a lot of learning resources I've used always recommend the **mobile first** approach.
- `margin-top: auto;` is always computed to 0 as specified by W3C “If “margin-top” or “margin-bottom” is “auto”, their used value is 0″. So it desn't work to center elements vertically which isn't so weird considering that working with heights is fundamentally different from working with widths in CSS.

I did not design this myself; however, it was fun to implement and solve some situations I ran into.
Credits to [Layo's Success](https://dribbble.com/shots/16769919-Online-education-platform) design.
