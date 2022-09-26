# Functions

## Tips
- :white_check_mark: Name should represent what it does
- :white_check_mark: Parameters should be self-describing
- :warning: Avoid `loops` and `if` nesting
- :no_entry_sign: Should not define unused parameters
- :no_entry_sign: Implementation should not be too long
- :no_entry_sign: Do not mix abstractions
    - either do/calculate something yourself, or orchestrate what other components do... not both.

## Examples
|:white_check_mark:|:no_entry_sign:|
|-|-|
|`double calculateCircleArea(double radius) => pi * radius * radius;`|`double a(double x) => pi * x * x;`|
|`void changePassword(String oldPassword, String newPassword) {};`|`void changePassword(String oldPassword, String newPassword, String address) {};`|
