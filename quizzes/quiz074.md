# quiz 074

```.py
def parity_check(msg: str) -> bool:
    ones = msg.count('1')
    bit = int(msg[-1])
    exp_bit = 1 if ones % 2 == 0 else 0
    if bit == exp_bit:
        return True
    else:
        return False
msgone = "100111001011001110010110011100101"
print(parity_check(msgone))

msgtwo = "011101111011101111101111001111"
print(parity_check(msgtwo))

```
**proof**
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2011.24.50.png)
![]()
