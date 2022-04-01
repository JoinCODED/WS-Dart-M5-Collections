You can use the `for-in` loop that we learned before to iterate over a map:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };

    for (var item in person){

    }
}
```

Oops we got an error:

```
The type 'Map<String, dynamic>' used in the 'for' loop must implement Iterable
```

To understand this message we need to know what an `Iterable` is:

Iterable is a collection of items that can be accessed `sequentially`.

according to this definition, both sets and lists are iterables and can use a `for-in` loop, but maps aren't, to get around this, we can iterate over only the keys of a map, which is a set of strings!

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };

    for (var key in person.keys){
        print(key);
    }
}
```

Output:

```
name
age
height
```

And to get the values we can:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };

    for (var key in person.keys){
        print(person[key]);
    }
}
```

Output:

```
salem
24
1.78
```

Another way to iterate over maps is to iterate over the `entries`:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };

    for (var entry in person.entries){
        print('${entry.key}: ${entry.value}');
    }
}
```

Output:

```
name: salem
age: 24
height: 1.78
```
