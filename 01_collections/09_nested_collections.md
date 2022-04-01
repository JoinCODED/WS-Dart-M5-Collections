Now that you know how to deal with sets, lists and maps, let's combine them together:

Suppose we have a list of movies:

```
name: Spider-man
ratings: [5.0, 3.5, 4.5]

name: Frozen
ratings: [5.0, 4.5, 4.0]

name: Twilight
ratings: [0.0, 0.5, 0.0]
```

Here, we can use a list of maps to represent this movies list:

```dart
void main() {
 var movies = [
     {
         'name': 'Spider-man',
         'ratings': [5.0, 3.5, 4.5]
     },
     {
         'name': 'Frozen',
         'ratings': [5.0, 4.5, 4.0]
     },
     {
         'name': 'Twilight',
         'ratings': [0.0, 0.5, 0.0]
     },
 ];
}
```

Now, we can iterate using `for-in` loop:

```dart
void main() {
 var movies = [
     {
         'name': 'Spider-man',
         'ratings': [5.0, 3.5, 4.5]
     },
     {
         'name': 'Frozen',
         'ratings': [5.0, 4.5, 4.0]
     },
     {
         'name': 'Twilight',
         'ratings': [0.0, 0.5, 0.0]
     },
 ];

 for(var movie in movies){
     print(movie);
 }
}
```
