To iterate over a `Map`, you can use the `for-in` loop that we learned before :

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };

    for (var item in person){
        print(item)
    }
}
```

Oops, we got an error:

```
The type 'Map<String, dynamic>' used in the 'for' loop must implement Iterable
```

To understand the message above, we need to know what an `Iterable` is:

As we mentioned in the beginning of this module, iterable is a collection of items that can be accessed `sequentially`.

According to this definition, both `Sets` and `Lists` can use a `for-in` loop, but `Maps` cannot. To get around this, we can iterate over the keys of a `Map` only, which is a set of strings.

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
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

To get the values, we can use the key surrounded by square brackets :

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
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
Salem
26
1.78
```

Another way to iterate over `Map` is to iterate over the `entries`:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
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
name: Salem
age: 26
height: 1.78
```
