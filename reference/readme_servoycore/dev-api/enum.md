# enum

A enum type is used for constants properties. That defines mostly a set of properties that belong to each other.

This can be used in plugins or in standard servoy api, the enum type is more typed so it shows in the javascript completion like: `enum<SomeType>`

This way the constants are typesafe. You can only drop a constant defined as `enum<SomeType>` in parameter of a **method that has that exact enum type** like `SomeType.UPDATE`, `SomeType.DELETE` which are `enum<SomeType>` but `AnotherType.UPDATE` <mark style="color:red;">**doesn't match**</mark>.


