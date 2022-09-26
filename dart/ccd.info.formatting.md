# Formatting

## Tips
- :white_check_mark: Use indentation
- :white_check_mark: Keep indentation consistent (e.g. tabs or spaces, spaces count)
- :no_entry_sign: Do not write multiple instructions in a single line
- :white_check_mark: Structure the content of a scope with new lines, similar to paragraphs separation
- :white_check_mark: Define parameters in new lines if neccessary
- :white_check_mark: Break arguments passing into new lines if necessary
- :white_check_mark: Split chained calls into separate lines
- :no_entry_sign: Do not mix styles of a single definition/call:
    - if some parameters/arguments are split into separate lines, keep them all that way
- :white_check_mark: Maintain the existing formatting style rules of your project or team:
    - eg.: whether or not opening brace `{` should be in a new line
    - eg.: whether tab or spaces should be used for indentation
    - eg.: how many character (at maximum) should a single line consist of
    - eg.: how long should functions be (at maximum)
- :no_entry_sign: Do not violate projects formatting style
- :white_check_mark: In a class it might be good to keep constructors first, then public methods and then private ones
- :no_entry_sign: Do not mix class methods & properties (i.e. keep all properties together and all methods together)
- :white_check_mark: There are tools that automate formatting checks which you can use (eg. [lints](https://pub.dev/packages/lints) or [flutter_lints](https://pub.dev/packages/flutter_lints))

## Examples

---

:white_check_mark:
```dart
void someFunction() {
    var exampleVariableInFunctionBody = 1;
}
```

:no_entry_sign:
```dart
void someFunction(){var exampleVariableInFunctionBody=1;}
```

---

:white_check_mark:
```dart
int calculateSomething(int a, int b, int c, int d) {
    final abDiff = a-b;
    final cdSum = c+d;
    final result = abDiff * cdSum;
    return result;
}
```

:no_entry_sign:
```dart
int calculateSomething(int a, int b, int c, int d) {
    final abDiff = a-b; final cdSum = c+d; final result = abDiff * cdSum;
    return result;
}
```

---

:white_check_mark:
```dart
int calculateSomething(int a, int b, int c, int d) {
    final abDiff = a-b;
    final cdSum = c+d;
    final result = abDiff * cdSum;
    return result;
}
```

:no_entry_sign:
```dart
int calculateSomething(int a, int b, int c, int d) {
       final abDiff = a-b;
    final cdSum = c+d;
     final result = abDiff * cdSum;
  return result;
}
```

---

:white_check_mark:
```dart
void someFunction() {
    prepareSomething1();
    prepareSomething2();
    prepareSomething3();

    performAction1();
    performAction2();

    cleanup();
}
```

:thinking:
```dart
void someFunction() {
    prepareSomething1();
    prepareSomething2();
    prepareSomething3();
    performAction1();
    performAction2();
    cleanup();
}
```

---

:white_check_mark:
```dart
return SomeWidget(
    child: const Text("abc")
);
```

:white_check_mark:
```dart
return SomeWidget(child: const Text("abc"));
```

---

:white_check_mark:
```dart
return SomeWidget(
    child: const Text(
      "abc",
      textAlign: TextAlign.center,
      overflow: TextOverflow.ellipsis
    )
);
```

:no_entry_sign:
```dart
return SomeWidget(child: const Text("abc", textAlign: TextAlign.center, overflow: TextOverflow.ellipsis));
```

---

:white_check_mark:
```dart
return users
    .expand((user) => user.moviesWatched)
    .toSet() // distinct
    .where((movie) => movie.genree == Genree.horror)
    .where((movie) => movie.rating > 3.5)
    .toList()
    ..sort((movie1, movie2) => movie1.year.compareTo(movie2.year));
```

:no_entry_sign:
```dart
return users.expand((user) => user.moviesWatched).toSet().where((movie) => movie.genree == Genree.horror).where((movie) => movie.rating > 3.5).toList()..sort((movie1, movie2) => movie1.year.compareTo(movie2.year));
```

---
