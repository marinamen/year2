# quiz 073

```.py
def check_message(message):
    num = 0
    for i in range(1, len(message)):
        num += 1
    return num % 2 != int(message[0])

print(check_message('111'))

```
