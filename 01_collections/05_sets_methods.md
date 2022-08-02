We learned about operations that can be done on both `Sets` and `Lists`. However, there are some unique methods that only work with `Sets`.


Assume that we have the two `Sets` below:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
}
```

Our first method is `.union()`, which combines two `Sets` and removes duplicates:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.union(vegetarianFood));
}
```

Output:

```
{vegetables, fruit, seeds, eggs, milk}    
```

Next, we have the `.intersection()` method, which generates a `Set` with only the items that are in both `Sets`:

```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.intersection(vegetarianFood));
}
```

Output:

```
{vegetables}
```

Lastly, we have the `.difference()` method, which generates a `Set` with the items that are in the first `Set`, but not in the second:
                                            
```dart
void main() {
    var veganFood = {'vegetables','fruit','seeds'};
    var vegetarianFood = {'vegetables','eggs','milk'};
    print(veganFood.difference(vegetarianFood));
}
```

Output:

```
{fruit, seeds}
```
