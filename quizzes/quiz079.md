# quiz 079
```.py
def calculate_parity(msg):
    p = 0
    while (2 ** p) < (len(msg) + p + 1):
        p += 1
    return p

def hamming(msg):
    parity_count = calculate_parity(msg)
    total_len = len(msg) + parity_count
    flist = ['_'] * total_len
    j = 0
    for i in range(1, total_len + 1):
        if (i & (i - 1)) == 0:
            flist[i - 1] = '-1'
        else:
            flist[i - 1] = msg[j]
            j += 1
    for i in range(parity_count):
        parity_pos = 2 ** i
        parity = 0
        for j in range(1, total_len + 1):
            if j & parity_pos:
                if flist[j - 1] != '-1':
                    parity ^= int(flist[j - 1])
        flist[parity_pos - 1] = str(parity)

    return ''.join(flist)

msg = '1011'
encoded = hamming(msg)
print(f'encoded string: {encoded}')


```

**proof**

![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2011.33.53.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2011.34.01.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2011.34.16.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_0258.jpg)
