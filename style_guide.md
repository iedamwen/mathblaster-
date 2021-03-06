# Team 04 Style Guide

This guide is designed to explain and set forth coding conventions and styles, as well as other guidelines for ensuring a uniform, easy to understand style for coding.

## Naming Conventions

#### Classes
- All classes shall use `UpperCamelCase`.

#### Methods
- All method names shall use `lowerCamelCase`, and should describe what the method does in a clear and concise manner.
  - Good: `updatePosition()`
  - Bad: `updateThePlayerPosition()`
- Methods should be 50 lines or less. Certain circumstances may prompt for exceptions, however.
- The use of frequent helper method is encouraged.

#### Variables and Constants
- All variable names shall use `lowerCamelCase`.
- Private variables may not be initialized before the constructor.
- Constants shall use `UPPER_UNDERSCORE_CASE`.
  - Where necessary for constants to be accessed by only one class, they should be `private final`.
  - Where necessary for constants to be accessed by many classes, they should reside in the Constants class, named `public static final`.
    - To import constants from the Constants class, use `import static Constants.CONSTANT_NAME`, or rather, `import static Constants.*`.

## Layout

#### Indentation
- Indentation shall be in the form of tabs, 4 spaces in width.
- **⚠️WARNING!** If you are using Netbeans, please do the following to ensure indentation works correctly:
	1. Go to Tools > Options
	2. Go to Editor > Formatting
	3. Select "All Languages" from dropdown
	4. Uncheck "Expand Spaces to Tabs"
	5. Set tab width to 4, close and apply \
*If you do not do this, the indentation will not work correctly for everyone else!*

#### Spaces, Braces, Brackets, Parentheses
- Loops and statements shall use spaces between the variable and value.
  - Good: `for (int i = 0 ; i < 42 ; i++)`
  - Also good: `for(int i = 0; i < 42; i++)`
  - Bad: `for(int i=0;i<42;i++)`
- Braces shall follow the line after the code is entered on.
  - Example:
    ```
    public class Foo 
    {
        someCode
    }
- There shall be at least one blank line between each method in a class.

## Coding Practices

- Lambda functions are preferred to anonymous classes when possible.
- Anonymous objects are allowed and encouraged.
