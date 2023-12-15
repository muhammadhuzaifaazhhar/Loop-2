# Loop-2
def fibonacci_sequence(n):
    fib_sequence = [1, 1]  # Initialize with the first two numbers in the sequence

    for i in range(2, n):
        # Calculate the next number in the sequence using the Fibonacci formula
        next_number = fib_sequence[i - 1] + fib_sequence[i - 2]
        fib_sequence.append(next_number)

    return fib_sequence

def main():
    # Number of Fibonacci numbers to display
    n = 20

    # Calculate and display the first 20 numbers in the Fibonacci sequence
    fib_sequence = fibonacci_sequence(n)
    print("Fibonacci Sequence (First 20):", fib_sequence)

if __name__ == "__main__":
    main()
