Assume that we have the following code:

```dart
void main () {
    const days = ['sunday','monday','tuesday'];
    const extraDays = ['friday','saturday'];
}
```

Let's try combining the two lists above into one list:

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

What if we want the elements of the first list to be included in the second list as items, not as a nested list?

Here, the `spread` operator (...) comes to help us to spread those elements into our second list:

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
