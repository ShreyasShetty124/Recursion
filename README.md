def s(n):
    # Base cases
    if n == 1:
        return 1
    elif n == 2:
        return 2
    elif n == 3:
        return 3
    
    # List to store the sequence values
    sequence = [1, 2, 3]
    
    # Generate the sequence up to the nth value
    for i in range(4, n + 1):
        next_value = sequence[-1] + sequence[-2] + sequence[-3]
        sequence.append(next_value)
    
    # Return the nth value
    return sequence[n - 1]

# Input
number = int(input("Enter the number: "))
print(f"s({number}) = {s(number)}")
