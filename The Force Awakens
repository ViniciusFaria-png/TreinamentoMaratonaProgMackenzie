def main() -> str:
    row = input().split()
    shape_y = int(row[0])
    shape_x = int(row[1])

    content = []

    for i in range(shape_y):
        current_input = input().split()
        
        current_row = [int(x) for x in current_input]

        content.append(current_row)

    for y in range(1, shape_y-1):
        for x in range(1, shape_x-1):
            if content[y][x] == 42:
                total = content[y-1][x-1] + content[y-1][x] + content[y-1][x+1] + content[y+1][x-1] + content[y+1][x] + content[y+1][x+1] + content[y][x-1] + content[y][x+1]
                if total == 56:
                    return f'{y+1} {x+1}'
                
    return '0 0'

print(main())
