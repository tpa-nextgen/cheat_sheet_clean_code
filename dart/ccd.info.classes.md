# Classes

## Tips
- :white_check_mark: Name should represent what is its role
- :white_check_mark: Name should represent how the role is being fulfilled
- :white_check_mark: Classes should be small
- :white_check_mark: Follow the ___SOLID principles___
- :warning: Prefer composition over inheritance
- :no_entry_sign: Should not define unused method/fields
- :no_entry_sign: Should separate private and public methods/fields
- :no_entry_sign: Should not implement unnecessary interfaces
- :no_entry_sign: Do not mix abstractions (either do/calculate something or orchestrate things)

## Examples
|:white_check_mark:|:no_entry_sign:|
|-|-|
|`class Storage<Data> {}`|`class Storage<T> {}`|
|`class TrendingAlbumsWidget extends StatelessWidget {}`|`class Trending extends StatelessWidget {}`|
|`class FileStorage<Data> extends Storage<Data>`|`class MyStorage<T> extends Storage<T> {}`|