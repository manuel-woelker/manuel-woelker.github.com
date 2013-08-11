title: Easy Drive-by Patches
date: 2011-12-24 14:30
tags: [github, maven, debian]
---

I was recently creating some debian packages at work using the excellent [jdeb maven plugin](https://github.com/tcurdt/jdeb) written by by [Torsten Curdt](http://vafer.org/). I was really happy with how easy it was to get working debian packages built by our integration server. Unfortunately I ran into a small issue with the generated directories. Since the source was readily available on [github](https://github.com/) I could quickly discover that there was a simple off-by-one error at fault. Since I already knew exactly what the problem was, it was a simple matter to correct the error.

Checking out the source, and fixing the bug took me all of 10 minutes, including the accompanying unit tests. Granted, the fix itself was all of two characters, but thanks to the excellent github infrastructure ([pull requests](http://help.github.com/send-pull-requests/)), the whole process was simple and lightweight enough to do in passing. For me as a software developer it felt easier to just write a testcase and the bugfix rather than a bug report.

So instead of being hampered by the bug, I took the opportunity to contribute something back to the project, without spending a disproportionate amount of my time on shaving yaks. This kind of ad-hoc collaboration is a really powerful proposition for the open-source model of software development. Thanks to tools like maven, git and github the barrier to entry has been lowered significantly in the recent years by making it easy to become involved. So the next time you stumble over a bug I encourage you to try to take matters into your own hands, and submit a pull request. For a quick how-to have a look at [Submitting a drive-by commit to a GitHub project in under 5 minutes](http://weblogs.asp.net/jgalloway/archive/2011/06/17/submitting-a-drive-by-commit-to-a-github-project-in-under-5-minutes.aspx) by Jon Galloway.
