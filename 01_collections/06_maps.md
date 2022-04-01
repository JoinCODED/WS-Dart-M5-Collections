The last type of collections is maps, aka `dictionaries` in other programming languages.

A map is used to store a collection of `key-value` pairs.

for example, we have those key-value pairs:

```
name: salem
age: 26
height: 1.78
```

to define a map in dart with those key-value pairs:

```dart
void main () {
    var person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
}
```

Keys in dart should always be unique and keys in the example above are all of type string, while the values are in mixed types.

To explicitly tell dart what the type of keys and values this map has:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
}
```

Within angular brackets after the `Map` keyword, we write the keys type followed by a comma, followed by the type of the values, and in our case keys are strings and the values are dynamic because the may be int,double or a string.

To access a value withing this map, we can use the square brackets:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };

    print(person['name']);
}
```

Output:

```
salem
```

To set a value for a specific key:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
    person['age'] = 40;
    print(person);
}
```

Output:

```
{name: salem, age: 40, height: 1.84}
```

We can also add new keys and values to our map:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
    person['married'] = false;
    print(person);
}
```

Output:

```
{name: salem, age: 40, height: 1.84, married: false}
```
