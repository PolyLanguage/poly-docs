
# Math operators 
Available math operators is:
- `+` (Add) 
- `-` (Subtract) 
- `*` (Multiply) 
- `/` (Divide)
- `%` (Modulus) 
- `^` (Power) 
Using math operators you can do math with numbers (int and real):
```poly
int a = 2;
int b = a + 1 * 2; // 4
int c = b / 2; // 2
int d = (c + 3) % 2; // 1
int f = 2 ^ 3; // 8
```

Also you can use `+` operator to concatenate strings:
```poly
string hello = 'hello' + ' ' + 'world';
print(hello + '!'); // hello world! 
```

Or concatenate arrays:
```poly
array<int> arr1 = [ 1, 2, 3 ];
array<int> arr2 = [ 4, 5, 6 ];
print(arr1 + arr2); // [ 1, 2, 3, 4, 5, 6 ] 
```

# Logical operators
Available logical(boolean) operators is:
- `&&` (And) 
- `||` (Or)
- `==` (Equals) 
- `!=` (Not Equals) 
- `<` (Less than) 
- `<=` (Less than or equals) 
- `>` (More than) 
- `>=` (More than or equals) 
All of the logical expressions always returns boolean value (true/false). 
First two operators is applied to booleans, the next ones to numbers. 
The equals/not equals operators can be applied to any types of values. 
Example:
```poly
print(2 == 2); // true
print(2 != 2); // false
print(2 < 2); // false
print(2 <= 2); // true
print(2 > 2); // false
print(2 >= 2); // true
```

Example of using 'and' and 'or' operators:
```poly
print(true || false); // true
print(true && false); // false
print(2 < 3 || 4 > 2); // true (2 less than 3 OR 4 more than 2)
print(2 <= 2 && 4 < 10); // true (2 less than or equals 2 AND 4 less than 10)
```
