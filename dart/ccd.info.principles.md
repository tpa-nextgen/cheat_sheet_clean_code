# Principles

## Well-known

### ___DRY___

Stands for ___Do not Repeat Yourself___.

It aims to reduce code repetitions. Whenever you start writting or copying the same code in various places, it is a good indicator to create function or class out of that functionality.

### ___KISS___

Stands for ___Keep It Simple, Stupid___.

It aims to pinpoint that the simple code is more desired than a complicated one.

### ___YAGNI___

Stands for ___You Ain't Gonna Need It___.

Showcases that only the code that is actually required should be written. In other words: do not implement features that you do not need right now.

### ___SOLID___

Set of five principles of object-oriented programming. Each letter of the acronym is the starting letter of the principle it is representing.

|Principle|Description|
|-|-|
|***S***ingle responsibility|Class should have only one responsibility and reason to change.|
|***O***pen-close|Open for extension. Closed for modification.|
|***L***iskov substitution|If a function works on a base class, it should also work on derived classes with no additional work or differentiation.|
|***I***nterface segregation|Interfaces should be minimal for any given usecase. No module should be forced to use interface that it is not fully utilizing.|
|***D***ependency inversion|High-level modules should be independent of low-level modules. Both should use & depend on abstractions. Concrete implementations should depend on abstractions.|

## Additional tips
- :white_check_mark: Prefer composition over inheritance
- :white_check_mark: Establishing common coding-style for a team or a project
- :white_check_mark: Keep a glossary of domain-specific names and abbreviations
- :white_check_mark: Use language, IDE or other automated solutions to effortlessly safe-check main coding style rules
- :white_check_mark: Implement unit tests
- :white_check_mark: Use code-reviews
- :white_check_mark: Resolve code warnings
- :white_check_mark: Create abstractions for used libraries to loosen dependencies