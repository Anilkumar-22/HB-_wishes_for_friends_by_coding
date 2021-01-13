for r in range(0,7):
    for c in range(0,11):
        if((c == 0) or( c == 4 and r != 3) or (r == 3 and(c ==2 or c == 1 or c == 3))): 
            print('-',end = " ")
        elif (c == 7 or (c == 8 and r%3 == 0) or (c == 9 and r%3 == 0) or (c == 10 and r%3 != 0)):
            print('+',end = " ")

        else :
            print(end = "  ")
    print()

print()
print()
for r in range(0,7):
    for c in range(0,27):
        if ((r == 0 and c%3 != 0) or (r == 1 and c%3 == 0) or (r + c == 8 and r != 6 and r != 5) or (r - c == 2 and r != 6 and r != 5) or (r == 6 and c == 3)):
            if c < 7:
                print('❣',end = ' ')
        elif ((c == 14 and (r%2 == 0 or r == 3 ) and r != 0 ) or (c == 15 and (r%2 == 0 and r != 0)) or ( c == 16 and(r%2 == 0 or r == 5 ) and r != 0)):
            print('S',end = ' ')
        elif ( c== 18 and r > 2):
            print('|',end = ' ')
        elif ((c == 20 and (r == 3 or r == 4 or r == 6)) or (c == 21 and (r == 3 or r == 5 or r == 6))):
            print('S',end = ' ')
        elif ((c == 23 and r == 3) or (c == 24 and(r == 4 or r == 6)) or (c == 25 and(r ==  4 or r == 5))or (c == 26 and r == 3)):
            print('~_~',end = ' ')
        else :
            print(end = '  ')
    print()
print()
print()
