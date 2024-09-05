```.py
def position_message(positions,msg,n):
  m=0
  final_msg=[]
  for i in range(k+n):
    final_msg.append(-1)
    if not in i positions:
      total_msg[i]=msg[x]
      x+=1
```


# OR

```.py
def position_message(positions, msg, n):
    k = calculate_parity(n)
    msg_list = [] 
    for i in range(len(k) + n):
        if i in k:
            msg_list.append(-1)  # Parity position, append -1
        else:
            msg_list.append(msg[i - len([p for p in k if p <= i])])
    return msg_list

```
        
