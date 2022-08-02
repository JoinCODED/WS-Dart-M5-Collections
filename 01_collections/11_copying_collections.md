Copying collections can be a bit confusing, let me demonstrate it:

```dart
void main() {
    final list = [1,2,3];
    final copy = list;

    copy[1] = 5;
    print('list: $list');
    print('copy: $copy');
}
```

What do you expect the output to be?

Output:

```
list: [1,5,3]
copy: [1,5,3]
```

This is strange, we only changed the second element of the `copy` list to `5`, but it changed in both lists, so what' i's going on?

When we create a list, Dart allocates a place in memory to contain these values. When we assign these to a variable, Dart will associate that variable with that reference in the memory that contains these values.
If we want, we can create more than one variable that point into the same values in the memory, like we did in the `list` and `copy`. Both are pointing to the same place in memory, that's why if we modify one, it will affect both variables.

So how do we make an actual copy? We can use the `spread` operator:

```dart
void main() {
    final list = [1,2,3];
    final copy = [...list];

    copy[1] = 5;
    print('list: $list');
    print('copy: $copy');
}
```

Output:

```
list: [1,2,3]
copy: [1,5,3]
```
