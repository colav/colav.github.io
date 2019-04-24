---
title: Development Guide
layout: content
toc: true
---

<center>
<img src="/img/PH-ROOT-icons-DG.png"/>
</center>

* Table of Contents 
{:toc}
<br>

# Colav Organization
<br/><br/>
<center>
<img src="/img/ColavDiagram.png" width="80%"/>
</center>
<br/><br/>



# Contributing
If you want to contribute read carefully this guide and lets to create a fork [https://help.github.com/articles/fork-a-repo/](https://help.github.com/articles/fork-a-repo/)
of our repositories, after you made your changes lets to create a Pull Requests [https://help.github.com/articles/about-pull-requests/](https://help.github.com/articles/about-pull-requests/)
After a Pull Requests is made, a set of automatic tests will be execute in Travis-CI and Codacy, you shuold to fix the problems and pass the review to merge the code.

# Coding Conventions
To write a high quality software Colav have a coding conventions 
that is based in Python PEP 8 Guide please read it carefully. [https://www.python.org/dev/peps/pep-0008/](https://www.python.org/dev/peps/pep-0008/)


# VCS - Git/Github
All our code is manipulate with a ditributed VCS(Version Control System) called git and hosted in 
in a cloud platform called [http://github.com](http://github.com) that lets do visualization of the code easily. 
Lets open a free account and see the documentation at [https://guides.github.com/](https://guides.github.com/) and [https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) 

# Documentation
The documentation is using PEP8 guidelines [https://www.python.org/dev/peps/pep-0008/#documentation-strings](https://www.python.org/dev/peps/pep-0008/#documentation-strings), 
please comment all with spaecial focus on classes, funcions and methods.
Example.
'''.py
def myfunction(arg1, arg2):
    """
    Method or function to do something.
    
    Parameters:
    ----------
    arg1: needed for X reason
    arg2: needed for Y reason
    """
    
    Returns:
    -------
    samples : the result of some procedure
    
    See Also
    --------
    myotherfunction : function to do other thnink
    
    Examples:
    --------
    >>> out = myfunction(arg1,arg2)
'''

<br/><br/><br/>
# Build Monitoring Tools
* Travis CI
* Codacy

