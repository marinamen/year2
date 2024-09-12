# quiz080
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_96FF96261163-1.jpeg)
```.py
def F(N:list):
    if len(N) == 1:
        return N[0]
    else:
        M = F(N[1:])
        if N[0] > M:
            return N[0]
        else:
            return M
```
**proof**
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2023.24.44.png)
