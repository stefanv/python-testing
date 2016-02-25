---
layout: page
title: Testing
---

> ## Prerequisites {.prereq}
>
> In this lesson we use a Python package called nosetests to find and execute
> tests.  Basic understanding of python variables and functions are a
> necessary prerequisite.  Some previous experience with the shell is
> expected, *but isn't mandatory*.

> ## Getting ready {.getready}
>
> Nothing to do: you're ready to go!

## Topics

1.  [Basics of Testing](01-basics.html)
2.  [Assertions](02-assertions.html)
3.  [Exceptions](03-exceptions.html)
4.  [Unit Tests](04-units.html)
5.  [Running Tests with Nose](05-nose.html)
6.  [Edge and Corner Cases](06-edges.html)
7.  [Integration and Regression Tests](07-integration.html)
8.  [Continuous Integration](08-ci.html)
9.  [Test Driven Development](09-tdd.html)
10. [Fixtures](10-fixtures.html)

Before relying on a new experimental device, an experimental scientist always
establishes its accuracy. A new detector is calibrated when the scientist
observes its responses to known input signals. The results of this
calibration are compared against the _expected_ response. **An experimental
scientist would never conduct an experiment with uncalibrated detectors -
that would be unscientific. So, too, simulations and analysis with untested
software do not constitute science.**

> ## How Do You Know Whether Your Code Functions Correctly? {.callout}
>
> **You can only know by testing it well.** Software bugs hide even in the
> most trivial software.  Testing is the process by which those bugs are
> systematically identified and exterminated--hopefully before causing a
> system failure, paper retraction, or worse.  Software tests, like
> device calibration, compare expected results against observed results in
> order to establish accuracy. 

The collection of all tests for a given piece of code is known as the _test
suite_. You can think of the test suite as a bunch of pre-canned experiments
that anyone can run. If all of the entire test suite passes, then the code is
at least partially trustworthy. If any test fails, then either the code or the
test itself is broken for that specific case.  After this lesson, you will
know not to trust software for which a) the test suite fails or b) the tests
do no _cover_ its full range of capabilities.

> ## But How Close is Close Enough? {.callout}
>
> In the same way that your scientific domain has expectations concerning 
> experimental accuracy, it likely also has expectations concerning allowable 
> computational accuracy. These considerations should surely come into play 
> when you evaluate the acceptability of your own or someone else's software.

In many programming endeavors, code can be fundamentally wrong -- even for
many years -- with minimal impact.  Perhaps a website goes down, or a game
crashes, or a day's worth of writing is lost due to a bug in your word
processor.  Scientific code, on the other hand, controls planes, weapons
systems, satellites, agriculture, and scientific simulations and experiments.
If the software that governs a simulation is wrong, e.g., a false claim in a
publication can be catastrophic to the author's career and even tarnish the
reputation of their field.

This is not to say that scientists have a monopoly on software testing, simply
that software cannot be called _scientific_ unless it has been validated.

> ## Why Untested Code is Legacy Code {.callout}
>
> In *[Working Effectively with Legacy
> Code](http://www.amazon.com/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052/)*,
> Michael Feathers defines legacy code as "any code without tests". This
> definition draws on the fact that, after its initial creation, tests provide
> a powerful guide to other developers (and to your forgetful self, a few
> months into the future) about how each function is meant to be used. Without
> runnable tests to provide examples of code use, maintaining even brand new
> programs quickly becomes unsustainable.

Testing is the calibration step of the computational simulation and analysis
world: it lets the scientist trust their own work on a fundamental level and
helps others to understand and trust their work as well.  Furthermore, tests
ensure that you never have to fix a bug a second time. Once a bug has been
caught and a test has been written, that particular bug can never again
re-enter the codebase unnoticed.  This also makes it a lot easier to rewrite
substantial portions of the system without fear of breaking related pieces of
code.  Whether motivated by principles or a desire to work more efficiently,
all scientists can benefit from testing.

> ## Effective Computation In Physics {.callout}
>
> Note that this testing lesson was adapted from the Testing chapter in 
> *[Effective Computation In Physics](http://physics.codes)*
> by Anthony Scopatz and Kathryn Huff.
> It is often quoted directly.


## Other Resources

*   [Reference](reference.html)
*   [Discussion](discussion.html)
*   [Instructor's Guide](instructors.html)
