If we have the following code:

```dart
void main () {
    const days = ['sunday','monday','tuesday'];
    const extraDays = ['friday','saturday'];
}
```

Let's try to combine those two lists into one list:

```dart
void main () {
    const days = ['sunday','monday','tuesday'];
    final extraDays = ['friday','saturday',days];
    print(extraDays);
}
```

Output:

```
['friday','saturday',['sunday','monday','tuesday']]
```

But what if we wan't the elements of the first list to be included in the second list as items not as a nested list, we can use the `spread` operator (...) to spread those elements into our second list:

```dart
void main () {
    const days = ['sunday','monday','tuesday'];
    final extraDays = ['friday','saturday', ...days];
    print(extraDays);
}
```

Output:

```
['friday','saturday','sunday','monday','tuesday']
```
