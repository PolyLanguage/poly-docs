# Using
To start programming with **Poly** you have multiple ways to work:
1. With *Poly Editor*
2. With *Poly CLI*

## With Poly Editor
1. Click "New Project" on the start page
2. Choose "Command Line Project" project type and click "Next" 
3. Choose name of your project and click "Create" 
4. You can start programming in the `main.poly` file
5. Click *Project > Run* or *F5* to launch your project
To build your project as Windows executable click *Project > Build*

## With Poly CLI
1. Create folder for your project
2. Create `main.poly` file inside
3. Write simple program code in `main.poly` file:
```c#
namespace 'MyProgram';

class Program
{
    method Main(array<string> args) {
        print('hello world');
    } 
} 
```
4. Run your project with command line:
```
poly run -project './' -debug
```

Also you can convert your project to Windows executable with command line:
```
poly build -mode il -project './' -out './bin/Release.exe'
```
