# quiz 074

```.py
def parity_check(msg):
    n = 0
    for i in range(1, len(msg)):
        if msg[i] == '1':
            n += 1
    return n%2 == int(msg[0])

msgone = "100111001011001110010110011100101"
print(parity_check(msgone))

msgtwo = "011101111011101111101111001111"
print(parity_check(msgtwo))

```
**proof**
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2022.59.45.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_983E59E2A7F9-1.jpeg)
