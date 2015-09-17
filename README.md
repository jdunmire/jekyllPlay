# jekyllPlay
Experiments with a static website

After looking through the sample themes (see below) I selected 
  * [slim pickens](http://chrisanthropic.github.io/slim-pickins-jekyll-theme/#toggleMenu)
  * [Code Folio](http://tokkonopapa.bitbucket.org/)
  * [mdl-jekyll](http://getaclue.github.io/mdl-jekyll/)

for further evaluation. I downloaded each of them and tried a sample
deploy. Code Folio hasn't been updated in 2 years, is missing
installation instructions, aside from using Prose.io. So I dropped it.

slim-pickens required a lot of extra ruby packages and the use of
rakefile. It isn't really designed for simple deployment on !GitHub. So
I dropped it.

mdl-jekyll worked, but the color scheme is garish to my eyes. I tried
the [custom theme builder](http://www.getmdl.io/customize/index.html)
but couldn't come up with anything much better.

Reading the [mdl-jekyll FAQ](http://www.getmdl.io/faq/index.html) I
concluded that this is still new with a lot of work-in-progress. It
replaces much of Bootstrap, but doesn't provide all the features. So I
conclude that if I'm going to use a style that is this heavy, I may as
well go with [solid](http://ojs.xyz/solid-jekyll/), which is Bootstrap.


## Themes I considered
I used the [Jekyll Themes
list](https://github.com/jekyll/jekyll/wiki/Themes) at
[GitHub](https://github.com) as the starting point and selected the
following for further consideration.

I am looking for a style to support a large project that will have
several parts: hardware design and documentation, firmware,
infrastructure software, and blog to keep track of what I've worked on.
Feedback and comments may become part of the project- it would be great
if I could interest others in the end product.

### [Incorporated](http://incorporated.sendtoinc.com/)
Pretty and eye-catching, but the top block is a sea of buttons. No clear
flow to where to start.  __DISCARDED__

### [Flex](http://the-development.github.io/flex/)
Clean and simple. Perhaps too simple. It is not clear where I can hook
in all the parts of a large project. __DISCARDED__

### [minimal mistakes](https://mmistakes.github.io/minimal-mistakes/)
Caught my eye, but on closer look this is primarily a blogging theme.
__DISCARDED__

### [solid](http://ojs.xyz/solid-jekyll/)
As it says, 'Eye-catching Bootstrap 3 Theme'. I do have some familiarity
with Bootstrap, so it is a contender. Initially DISCARDED, but in
the end this is my __selected starting theme__.


### [skinny bones](https://mmistakes.github.io/skinny-bones-jekyll/)
The use instructions appear to be good and there are lots of hooks for
menus, tables of content, and sub-sections. Ultimately __DISCARDED__
because of the edge-to-edge background image. Seems like a promotion for
a project more than documentation.


### [slim pickens](http://chrisanthropic.github.io/slim-pickins-jekyll-theme/#toggleMenu)
Most of the navigation is in the menu bar. Responsive grid and
navigation. Good integration with s3, but not as clear how to use it
with [GitHub](https://github.com).

Lots of great ideas and support for tasks- see the _rakefile_
documentation.


### [Code Folio](http://tokkonopapa.bitbucket.org/)
Nice use of grid. Multiple themes. On big screens the information from
several menu items is shown, on small screens only one category.

Blog entries seem to emphasize photography- at least there is photo
associated with each example post. Could be good or bad: nice place to
put a schematic, board layout, or other useful image, but could cause a
large waste of time selecting images.

Disqus section for comments on each blog post.

The source has not been updated in 2 years and there are no installation
instructions aside from using Prose.io

__DISCARDED__


### [mdl-jekyll](http://getaclue.github.io/mdl-jekyll/)
_Material Design Lite_, [(MDL)](http://www.getmdl.io/index.html), is part of the
[Google /Web tools](https://developers.google.com/web/tools/?hl=en)


## Other Notes
While the files in {{{gh-pages}}} are processed by Jekyll, if there are
no Jekyll directives, configurations, etc. they the files are served
un-modified (AFAICT). That means that any static generator could be used
and the results of the generation could be committed to the
{{{gh-pages}}} branch at which point they will be served by !GitHub.


