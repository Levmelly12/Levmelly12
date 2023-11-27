# Function to generate Fibonacci sequence up to n terms
generate_fibonacci <- function(n) {
  fibonacci_sequence <- numeric(n)
  
  # Base cases
  fibonacci_sequence[1] <- 1
  fibonacci_sequence[2] <- 1
  
  # Generate the Fibonacci sequence
  for (i in 3:n) {
    fibonacci_sequence[i] <- fibonacci_sequence[i - 1] + fibonacci_sequence[i - 2]
  }
  
  return(fibonacci_sequence)
}

# Generate Fibonacci sequence up to the 8th term
fibonacci_result <- generate_fibonacci(8)

# Print the result
print(fibonacci_result)
