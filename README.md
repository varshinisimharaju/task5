# task5
arr = [int(x) for x in input("Enter a list of integers separated by spaces: ").split()]

max_num = arr[0]
second_max = float('-inf')

for num in arr[1:]:
    if num > max_num:
        second_max = max_num
        max_num = num
    elif num > second_max and num != max_num:
        second_max = num
            
print(second_max)
