# Variables. Types
Poly is a static-typed programming language. It's means that every variable/constant/argument has type of the value, you cannot apply value of one type to value of another type, but you can convert values to other types. 

The default types of Poly language:
- `int` (Integer numbers)
- `real` (Float/Double numbers)
- `string` (Text)
- `bool` (Boolean values: `true` or `false`)
- `lambda` (Function)
- `array<T>` (List of values of `T` type, `T` may be any of available types)
- `object` (Dictionary values)
- `void` (The `null` value type)

# Variables. Syntax
To define a variable you simply specify it's type, name and the value that way:
```poly
class Program {
    method Main(array<string> args) {
        // Variable with integer type, name x and the value 1
        int x = 1;
        print(x); // 1

        real y = 2.2;
        print(y); // 2.2

        string z = 'hello world!';
        print(z); // hello world!

        bool w = true;
        print(w); // true
    }
}
```

Definition of variable is the statement, at the end of it you have to use semicolon (`;`). You can define a variables only inside methods/loops/conditions/blocks. 

# Variables. Lambda
Lambdas is basically methods values, you can define a method inline as lambda and use it or pass to other methods as argument. 
Example:
```poly
lambda mymethod = lambda() { print('Hello!'); };
mymethod();
```

If your lambda returns some value, you should specify return value of lambda:
```poly
lambda<int> sum = lambda int(int a, int b) { return a + b; };
print(sum(5, 5)); // 10
```

# Variables. Array
Array is a list of different values. Every array also has a type of its values `T`. Example of creating array of `int` values:
```poly
array<int> mylist = [1, 2, 3];
```

`T` type may be any type, it means you can specify `T` type as array and create 2D arrays:
```poly
array<array<int>> array2d = [
    [1, 2],
    [3, 4],
    [5, 6]
];
```

# Variables. Object
Soon.