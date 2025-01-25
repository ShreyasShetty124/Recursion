def s(n):
    if n == 1:
        return 1
    elif n == 2:
        return 2
    elif n == 3:
        return 3
    
    sequence = [1, 2, 3]
    
    for i in range(4, n + 1):
        next_value = sequence[-1] + sequence[-2] + sequence[-3]
        sequence.append(next_value)
    
   
    return sequence[n - 1]

number = int(input("Enter the number: "))
print(f"s({number}) = {s(number)}")
