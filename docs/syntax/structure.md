# Structure
The first thing you have to learn - is structure of Poly files. The top level statements is the:
- `import` statements
- `namespace` statement
- `class` declarations

### namespace
The must-have statement is the `namespace` which defines namespace of your file. When you will import that
namespace, all the classes in files with that namespace will be available for you to use. The `namespace` statement
looks like that:

```poly
namespace 'MyProgram';
```

Namespace name can only contain latin symbols, numbers and dots.

### import
The `import` statements allows to import specific namespace and use its classes inside your file. Statement is looks
like that:

```poly
import 'SomeNamespace';
```

### class
Also at the top level of the program you can define classes. In the *entrypoint* file you must define `Program` class
with the `Main` method which will be runned on your program launch. Example of `Program` class:

```poly
class Program
{
    method Main(array<string> args) 
    {
        // Write the code that will be runned at the program launch... 
    } 
} 
```

## Command line app
The structure of the command line app is simple. The entrypoint file should has `Program` class
with the `Main` method that may accept arguments:

```poly
namespace 'MyProgram';

class Program
{
    method Main(array<string> args) 
    {
        // Printing to the console
        print('Hello world!');
    }
} 
```

## WinForms app
The structure of WinForms app almost the same as command line app structure. Entrypoint file should
have `Program` class with the `Attributes` field and `Main` method:

```poly
// Importing WinForms
import 'WF';

namespace 'MyProgram';

class Program
{
    field array<int> Attributes = [WinForms.PROGRAM_ATTR];
    
    method Main(array<string> args) 
    {
        // Creating WinForms window
        Window window = Window.FromFile('windows/MainWindow.xaml');
        
        // Opening WinForms window
        window.Open();
        window.WaitForExit();
    }
} 
```
