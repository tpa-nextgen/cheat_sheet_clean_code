# Naming

## Tips
- :white_check_mark: Keep consistency (use the same name for the same meaning)
- :no_entry_sign: Do not use redundant names (different names for the same meaning)
- :white_check_mark: Use descriptive names (clear intentions):
    - variable name should indicate its content meaning
    - method name should describe clearly what it does
    - class/interface name should indicate what is its role
    - class that implements abstraction should indicate how it is doing so
- :no_entry_sign: Do not use names that mean nothing or are ambiguous
- :warning: Avoid unclear abbreviations
- :warning: Avoid using type name in variable name
- :white_check_mark: Keep a glossary of domain-specific names and abbreviations
- :white_check_mark: Vary name length based on clarity:
    - eg.: local & loop variables may be shorter
    - eg.: fields, properties and parameters may need be longer
- :white_check_mark: Use well-known standards
- :white_check_mark: Keep in sync with level of abstraction
- :warning: May be good to differentiate between naming of interfaces, abstract classes & concrete implementations
- :warning: Always pay attention to naming, it easily spreads across the codebase

## Examples
|:white_check_mark:|:no_entry_sign:|
|-|-|
|`login` ___or___ `signin`|`login` ___and___ `signin`|
|`var bottomBar = [home, podcasts, search, profile];`|`var hpsp = [tab1, tab2, tab3, tab4];`|
|`double calculateCircleArea(double radius) => pi * radius * radius;`|`double a(double x) => pi * x * x;`|
|`class Storage<Data> {}`|`class Storage<T> {}`|
|`class TrendingAlbumsWidget extends StatelessWidget {}`|`class Trending extends StatelessWidget {}`|
|`class FileStorage<Data> extends Storage<Data> {}`|`class MyStorage<T> extends Storage<T> {}`|
|`int dogsCount = 10;`|`int abcd = 10;`|
|`int dogsCount = 10;`|`int int_dogsCount = 10;`|
|`var peopleCount = 0;`|`var pplc = 0;`|
|`displayAsList(trending);`|`displayAsList(category2);`|
|`for (var tedTalk in tedTalks)`|`for (var x in list)`|
|`for(var i = 0; i < 10; i++)`|`for(var abc = 0; abc < 10; abc++)`|
|`Data readDataFrom<Source>(Source source) {}`|`Data readDataFrom<Source>(Source file) {;`|

---

|:heart_eyes_cat:|:thinking:|
|-|-|
|`abstract class AStorage<Data> {}`|`abstract class Storage<Data> {}`|
