# quiz076

```.py
def positions(k):
    pos=[]
    for i in range(k):
        pos.append((2**i)-1)
    return pos
n = 3
par_pos = positions(n)
print(par_pos)
def create(k, n):
    len=k+n
    array = [0]*len
    par_pos=positions(k)
    for pos in par_pos:
        array[pos] = 1
    return array

result = create(4, 7)
print(result)
```
**proof**
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2013.03.48.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2013.04.01.png)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2013.04.08.png)
