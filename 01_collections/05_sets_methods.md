We learned about operations that can be done on both sets and lists, but we have some unique methods that only works with sets:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
}
```

Our first method is `union()` which combines 2 sets and removes duplicates:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.union(vegetarianFood));
}
```

Output:

```
vegetables, fruit, seeds, eggs, milk
```

Next, we have the `intersection()` method, that generate a set with only the items that are in both sets:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.intersection(vegetarianFood));
}
```

Output:

```
vegetables
```

Lastly, we have the `difference()` method, which generates a set with the items that is in the first set, but not in the second:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.difference(vegetarianFood));
}
```

Output:

```
fruit, seeds
```
