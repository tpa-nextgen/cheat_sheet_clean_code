# Classes

## Tips
- :white_check_mark: Name should directly indicate purpose / role / responsibility
- :white_check_mark: Name should represent how the class is being implemented (e.g. include official algorithm name)
- :white_check_mark: Classes should tend to be small (e.g. don't mix functionalities, keep it compact)
- :white_check_mark: Follow the [___SOLID principles___](./ccd.info.principles.md#SOLID)
- :warning: Prefer [composition](https://en.wikipedia.org/wiki/Object_composition) over inheritance
- :no_entry_sign: Should not define unused method/fields
- :no_entry_sign: Should separate the locations of private and public methods/fields (e.g. keep private fields after public fields, private methods after public methods)
- :no_entry_sign: Should not implement unnecessary interfaces
- :no_entry_sign: Do not mix abstractions (either do/calculate something or orchestrate things)

## Examples
|:white_check_mark:|:no_entry_sign:|
|-|-|
|`class Storage<Data> {}`|`class Storage<T> {}`|
|`class TrendingAlbumsWidget extends StatelessWidget {}`|`class Trending extends StatelessWidget {}`|
|`class FileStorage<Data> extends Storage<Data> {}`|`class MyStorage<T> extends Storage<T> {}`|
