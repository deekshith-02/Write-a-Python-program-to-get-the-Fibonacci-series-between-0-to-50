# Write-a-Python-program-to-get-the-Fibonacci-series-between-0-to-50
def fibonacci_series(n):
    fib_series = [0, 1]  # Initialize the Fibonacci series with the first two numbers

    while True:
        next_num = fib_series[-1] + fib_series[-2]  # Calculate the next number in the series
        if next_num > n:
            break
        fib_series.append(next_num)

    return fib_series


# Example usage
fibonacci_numbers = fibonacci_series(50)
print("Fibonacci series between 0 and 50:")
print(fibonacci_numbers)
