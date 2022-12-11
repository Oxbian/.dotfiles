# Intro

It's important to choose a coding style, so for this reason I decide to write it in a file to force myself to respect it.

# Inspiration

My coding style is inspired by:

- https://www.kernel.org/doc/html/v4.10/process/coding-style.html
- https://docs.unrealengine.com/en-US/Programming/Development/CodingStandard
- https://webkit.org/code-style-guidelines/

# General rules

## Readability and Simplicity first

Your code is intended to be read.
Avoid one-liners from hell and keep code complexity under control.
Try to make code self explanatory and add comments if needed.
Leave references to standards that you are implementing.


## Variable and function names must clearly define what it's doing

It's ok if it will be long, but it should clearly state what it's doing, without need to dive into code.
This also applies to function/method's code.
Try to avoid one letter variables.

## Encapsulation

Don't expose raw data, provide methods to work with it.

# C coding style

- Tab is 4 spaces
- Use `Format` to reformat source code and check style guide before commit

## Naming

### Type names are CamelCase

Examples:

	HelloWorld
	MyCustomInt
	MyCustomFloat


### Functions are snake_case

	my_custom_int_init
	my_custom_int_delete
	hello_world_print

### File names

- Directories: `^[0-9A-Za-z_]+$`
- File names: `^[0-9A-Za-z_]+\.[a-z]+$`
- File extensions: `[ ".h", ".c", ".cpp", ".cxx", ".hpp" ]`

Enforced by linter.

### Standard function/method names

Suffixes:

- `alloc` - allocate and init instance. C style constructor. Returns pointer to instance.
- `free` - deinit and release instance. C style destructor. Takes pointer to instance.

# C++ coding style

Work In Progress. Use C style guide as a base.

# Python coding style

- Tab is 4 spaces
- Inspired by [black](https://pypi.org/project/black/) to reformat source code
