#MANAGING TECHNICAL DEBT IN (DJANGO) PROJECTS
[Talk repo](https://github.com/crccheck/tech-debt-talk)

##Tech debt is
-  Fixing one bug will create another
-  security patches may break something
-  "It works for me"

##Some tips for minimizing it
-  Testing in Django
    +  If you're making an assumption, you SHOULD be writing a test to CHECK that assumption
    +  EVEN if you scrimp on up-front testing, DO regression testing
-  [CI guide](http://docs.python-guide.org/en/latest/scenarios/ci/)
-  Code Quality
    +  Iterate for more practice. Practice makes perfect.
    +  Keep things simple. Code that requires less context to understand.

##Related topics
-  #nocomments
-  [cyclomatic complexity](https://en.wikipedia.org/wiki/Cyclomatic_complexity)
-  McDabe
-  Pep8
-  PyFlakes

##Code Review
-  [Raymond Hettinger: Beyond PEP8](https://www.youtube.com/watch?v=wf-BqAjZb8M)
-  Pair Programming: Best away to up code quality & share knowledge
    +  tmux + vam
    +  Driver + Navigator
    +  Ping pong pair programming
##Toyota Kata
http://www-personal.umich.edu/~mrother/Homepage.html

##Teams
-  Hire coworkers you get along with
    +  Diversity/inclusion issues?

##Feature Flip?
I need to learn more about this.

##Django Specific
-  Don't customize the Django admin. It's a dev interface, not a CMS.
-  Clean as you cook
-  Unique names: part of Django shell extensions
-  Avoid the Django test client
    +  DON'T use it for unit tests
    +  DO use it for Integration tests
-  Avoid model inheritance: hurts readability & performance
-  Stay Fresh
    +  requirements.txt; keep your version bumped up as often as you can
    +  Only works when you have test coverage

##The Phoenix Project
I HAVE THIS! As a Kindle book. Read it!

