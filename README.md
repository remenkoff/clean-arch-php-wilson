# The Clean Architecture in PHP
###### Practical part of the «The Clean Architecture in PHP» book by Kristopher Wilson.

## Intro
Methods in this book helps to make application:

1. Testable;
2. Refactorable;
3. Easy to work with;
4. Easy to maintain.

*The author prefers and suggests the use of
[PSR-2 coding standards](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md)*.

## The Problem with Code
Summarized:

- **writing good code is hard**: if it were easy to be good at it, everyone would be good at it;
- **writing bad code is easy**: too easy to find bad code in PHP; too easy to suggest (via putting source code out 
there or writing tutorials) others write bad code; too easy for developers to never “level up” their skills;
- **we can't test anything**: it is nearly impossible to test poorly written code;
- **change breaks everything**: regression bug — is a bug caused after introducing new features, fixing other bugs, 
upgrading a library, changing configuration settings, etc.;
- **we live or die by the framework**: when writing software within a framework, your code is so embedded into that 
framework that you’re essentially entering a long term contract with that framework; but there is a way to write code, 
using a framework, in such a way that switching out the framework shouldn’t lead to a complete rewrite of the 
application;
- **we want to use all the libraries**: if you’ve littered your code base with usages of some library, you now have 
a time consuming process to run through to upgrade your application to use some other library; adapters and a 
good-written test suite for them will guarantee a minimal amount of work and bugs, respectively, when the time comes to 
replace the libraries.
