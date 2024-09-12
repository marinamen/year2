# QUIZ 078


```.py
def insert_parity(msg, ham_pos, k):
    final = [-1 for _ in range(len(msg) + k)]
    msgindex = 0
    for i in range(len(final)):
        if i not in ham_pos:
            final[i] = msg[msgindex]
            msgindex += 1
    return final
msg='1011'
k=3
ham_pos=[0,1,3]

print(insert_parity(msg, ham_pos, k))

```


**proof**
        
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_5E03D09C5469-1.jpeg)
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-12%20at%2023.41.44.png)
