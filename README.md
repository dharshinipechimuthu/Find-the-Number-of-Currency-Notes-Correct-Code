# Find-the-Number-of-Currency-Notes-Correct-Code
def no_notes(a):
    Q = [500, 200, 100, 50, 20, 10]
    count = 0

    for q in Q:
        count += a // q
        a = a % q

    if a > 0:
        return -1
    return count

print(no_notes(500))
print(no_notes(560))

Output:
1
3
