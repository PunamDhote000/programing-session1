def sum_of_absolute_differences(arr):
    index_map = {}

    for i, num in enumerate(arr):
        if num not in index_map:
            index_map[num] = [i, i]  
        else:
            index_map[num][1] = i  

    return sum(abs(v[1] - v[0]) for v in index_map.values())

t = int(input().strip())  

for _ in range(t):
    n = int(input().strip())  
    arr = list(map(int, input().strip().split()))  

    print(sum_of_absolute_differences(arr))
