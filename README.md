# india_pattern_pythoncode
TO PRINT INDIA PATTERN USING PYTHON CODE
CODE:
def print_I(height):
    width = height // 2
    for i in range(height):
        if i == 0 or i == height - 1:
            print('*' * width)
        else:
            print(' ' * (width // 2) + '*')
    print()

def print_N(height):
    for i in range(height):
        print('*' + ' ' * i + '*' + ' ' * (height - i - 1) + '*')
    print()

def print_D(height):
    width = height // 2
    for i in range(height):
        if i == 0 or i == height - 1:
            print('*' * width)
        else:
            print('*' + ' ' * (width - 2) + '*')
    print()

def print_A(height):
    width = height // 2
    for i in range(height):
        if i == 0:
            print(' ' * (width // 2) + '*' + ' ' * (width // 2))
        elif i == height // 2:
            print('*' * width)
        else:
            print('*' + ' ' * (width - 2) + '*')
    print()

def print_india(height):
    print_I(height)
    print_N(height)
    print_D(height)
    print_I(height)
    print_A(height)

if __name__ == "__main__":
    predefined_height = 7  # Set a predefined height for the design
    print_india(predefined_height)
OUTPUT:
***
 *
 *
 *
 *
 *
***

**      *
* *     *
*  *    *
*   *   *
*    *  *
*     * *
*      **

***
* *
* *
* *
* *
* *
***

***
 *
 *
 *
 *
 *
***

 * 
* *
* *
***
* *
* *
* *
