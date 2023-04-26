# attiny44_adcs

`project`

The project uses an ATtiny44 microcontroller to communicate with sensors on board the CubeSat and to send data to the local station. The firmware is written in C and uses the Arduino framework under the hood with the PlatformIO IDE for project management.

### ©️ Copyright statement:
In this project, every mention of the word "author" refers to [Diego Anestor Coutinho](https://www.linkedin.com/in/diego-anestor-coutinho).  
All the code in this project is the exclusive property of the author and is protected by intellectual property laws. No part of this code may be copied, modified, distributed, or licensed without the prior written consent of the author. Any unauthorized use of this code will constitute a violation of the author's rights and may result in legal action.

---
### File structure:

- **`src`** folder:

The **src** folder contains the source code of the application. It usually has one or more .cpp or .c files that define the logic and functionality of the application. 

- **`lib`** folder

The lib folder contains the libraries that are used by the application. These can be either external libraries that are downloaded from the PlatformIO library registry or custom libraries that are written by the author. Each library should have its subfolder inside the lib folder. For example, a library called MyLib could have a folder called MyLib with the following files:

```
├── MyLib
    ├── MyLib.h
    ├── MyLib.cpp
```

The `MyLib.h` file could have the following content, with all the functions and class definitions, following recommended formatting and documentation:

```cpp
#ifndef MYLIB_H
#define MYLIB_H

#include <ArduinoJson.h>

// Class declaration
class MyLib 
{
    // Method declaration
    public:
    MyLib();
    void doSomething();
    private:
    JsonObject data;
};

#endif
```

The `MyLib.cpp` file could have the following content, with all the functions and class declarations, following recommended formatting and documentation:

```cpp
#include "MyLib.h"

MyLib::MyLib() 
{
    data = JsonObject();
}

void MyLib::doSomething() 
{
    // do something with the data
    // code is written here
}
```
  
- **`include`** folder

The included folder contains the header files that declare the functions and variables of the firmware and its libraries. These are usually C or C++ files with the .h or .hpp extensions. #include directives are used to include these files in the source code files. For example, a MyLib.h file in the include folder that declares a function of a library is usually written as:

```cpp
#ifndef MYLIB_H
#define MYLIB_H

// Simple function to return the sum of two numbers
int add(int a, int b)
{
    return (a + b);
}

#endif
```

Inside the `include` folder, numerical constants are generated to control data-position inside arrays. A *typedef enum* is a way of defining a new data type that consists of a set of named constants. 

```cpp
// color.h
#ifndef COLOR_H
#define COLOR_H

typedef enum {
    RED,
    GREEN,
    BLUE,

    YELLOW = 10,
    MAGENTA,
    CYAN
} color;

#endif
```

The example above gives the values RED = 0, GREEN = 1, BLUE = 2, YELLOW = 10, MAGENTA = 11, CYAN = 12, some assigned automatically.
This method can be used to control the position of variables inside arrays and constant values.