# india_pattern_pythoncode
code:def print_I():
    for i in range(5):
        for j in range(5):
            if i == 0 or i == 4 or j == 2:
                print("*", end="")
            else:
                print(" ", end="")
        print()


def print_N():
    for i in range(5):
        for j in range(5):
            if j == 0 or j == 4 or i == j:
                print("*", end="")
            else:
                print(" ", end="")
        print()


def print_D():
    for i in range(5):
        for j in range(5):
            if j == 0 or (j == 4 and (i != 0 and i != 4)) or (i == 0 or i == 4) and (j > 0 and j < 4):
                print("*", end="")
            else:
                print(" ", end="")
        print()


def print_A():
    for i in range(5):
        for j in range(5):
            if (j == 0 or j == 4) and i != 0 or (i == 0 or i == 2) and (j > 0 and j < 4):
                print("*", end="")
            else:
                print(" ", end="")
        print()


def print_space():
    for i in range(5):
        print(" ", end="  ")
    print()


def print_INDIA():
    print_I()
    print_space()
    print_N()
    print_space()
    print_D()
    print_space()
    print_I()
    print_space()
    print_A()


print_INDIA()

