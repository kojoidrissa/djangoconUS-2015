#[DJANGO VIEWS: FUNCTIONS, CLASSES, AND GENERICS](http://2015.djangocon.us/schedule/presentation/74/)
afrg.co/views ==> http://andrewsforge.com/presentation/django-views-functions-classes-generics/
afrg.co/dju
afrg.co/class (djangoconus ==> 20% off)

##fundamentals -> problem, solution
-  Python `callables`
    +  I need to learn the definition of this. Seems to be something I can call.
        +  https://docs.python.org/3.4/library/functions.html?highlight=callable#callable
    +  `__call__` method makes ANYTING callable
        *  https://docs.python.org/3.4/reference/datamodel.html#object.__call__
-  What is a view?
    +  Type of web page
    +  dynamic generation of content
    +  tied to URL patterns
-  ANY Python callable can be a view
-  State of the Pony 2015 re: Views
    +  Function Views
    +  Object Views(Class-based views)
    +  Generic (class-based) views

###Class Based Views
-  make your function-based view a METHOD of a class (with a few small changes)

###Generic Class-Based Views
-  Beginners shouldn't use these, unless there's one that does EXACTLY what you want.
-  stick to the basics
-  [Classy Class-Based Views](http://ccbv.co.uk/)

##Answers
-  Function views aren't going away because ANY callable can be a view
-  All class-based views are NOT generic
-  How do I choose which view to use?
    +  If generic view fits exactly, use
    +  If I need to inherit/share behaviour, use CBV
    +  Otherwise, use CBV or FUnction views
