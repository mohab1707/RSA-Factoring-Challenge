#!/usr/bin/env python3

import sys
import math

def factorize(number):
    """
    Factorize a number into a product of two smaller numbers.
    """
    for i in range(2, int(math.sqrt(number)) + 1):
        if number % i == 0:
            return i, number // i
    return number, 1  # If the number is a prime, return the number itself

def main():
    if len(sys.argv) != 2:
        print("Usage: {} <file>".format(sys.argv[0]))
        sys.exit(1)

    input_file = sys.argv[1]

    with open(input_file, 'r') as file:
        for line in file:
            number = int(line.strip())
            factors = factorize(number)
            print("{}={}*{}".format(number, factors[0], factors[1]))

if __name__ == "__main__":
    main()
