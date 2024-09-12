# quiz 073

```.py
def check_error(data):
    n=len(data) // 3
    o, c1, c2=data[:n], data[n:2 * n], data[2 * n:]
    err=False
    res=[]
    for i in range(n):
        if o[i]==c1[i] or o[i] == c2[i]:
            res.append(o[i])
        elif c1[i]==c2[i]:
            res.append(c1[i])
        else:
            res.append(c1[i])
        if o[i]!=c1[i] or o[i]!=c2[i]:
            err=True

    return res, err


data = '011101111101110111110111001111'
corrected, has_error = check_error(data)
print(f"{corrected}")
print(f"error: {has_error}")

```
**proof**

![](https://github.com/marinamen/year2/blob/main/quizzes/media/compsci.jpeg)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_0D3AAEA3BE89-1.jpeg)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2011.45.05.png)
