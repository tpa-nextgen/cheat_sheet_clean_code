# Comments

## Tips
- :no_entry_sign: Do not use comments as an excuse for poorly written code
- :no_entry_sign: Do not repeat what the code does
- :no_entry_sign: Do not explain variable names
- :white_check_mark: Use as last resort
- :white_check_mark: Use to expand the context:
    - Use to explain or clairify decisions
    - Use to explain edge case
    - Use to link external resource (eg. standard or algorithm theory)
- :white_check_mark: Use to mark things to be done (___TODO___ comment)
- :white_check_mark: Use to highlight what has been tried already to improve the function
- :white_check_mark: Use `///` (three-slash comments) to provide documentation of a class/function/property

## Examples
|:white_check_mark:|:no_entry_sign:|
|-|-|
|`}`|`} // close if bracket`|
|`var circleArea = r*r*pi;`|`var circleArea = r*r*pi; // calculate circle area`|
|`var minutes = 100;`|`var time = 100; //minutes`|
|`// See TCP (Transmission Control Protocol): https://datatracker.ietf.org/doc/html/rfc9293`|_no context_|
|`// TODO: Implement saving to the file`|_empty function_|
|`// Things that were already tried to optimize this function:`|_no comment_|

### :white_check_mark: Edge case & decision clarification example:
```java
final Object value = (new JSONTokener(jsonString)).nextValue();
// Note that JSONTokener.nextValue() may return
// a value equals() to null.
if (value == null || value.equals(null)) {
    return null;
}
```
