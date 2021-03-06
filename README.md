# stylus-csswizardry-grids

This is a port from Sass to **Stylus**.
There are two main differences from the original:

*	You don't have an option to set Stylus to use silent classes, because Stylus does that automatically when you @extend the class - you can read more about it [here](http://learnboost.github.com/stylus/docs/extend.html).
* Due to a [bug](https://github.com/csswizardry/csswizardry-grids/issues/4) with Google Chrome (release 25), I changed back the **grid__item** to use **float** instead of **inline-block**. It seems more reasonable than adding an empty comment after each **grid__item**.

**Simple, fluid, nestable, flexible, Stylus-based, responsive grid system.**

* Fully responsive
* Infinitely nestable
* Endless possible combinations
* Simple to understand, human-friendly classes
* Option to keep classes out of your HTML
* Robust
* Simple
* No `.clear` or `.last` classes
* It just _works_

Please see [Responsive grid systems; a solution?](http://csswizardry.com/2013/02/responsive-grid-systems-a-solution/)
for a comprehensive overview of the principles of the grid system.

## Setup

Simply fill in/adjust the relevant variables.

* `$gutter` controls how much space there is between columns.
* `$lap-start` and `$desk-start` tell csswizardry-grids when to fire particular
  media queries to service those particular sizes. Note that csswizardry-grids
  works out the ends of any other breakpoints by using these numbers.

## Basic usage

If you are using traditional classes then an example, basic usage might look
like this:

    <div class="grid">
    
        <div class="grid__item  lap-one-half  desk-two-thirds">
            ...
        </div>
    
        <div class="grid__item  lap-one-half  desk-one-third">
            ...
        </div>
    
    </div>

There is a very simple demo which can be found at
[csswizardry.github.com/csswizardry-grids](http://csswizardry.github.com/csswizardry-grids).
