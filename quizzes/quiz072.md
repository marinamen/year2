# quiz 072

*pseudocode*
```.py
DATA={"Ankara","Turkey","Tokyo","Japan","Lisbon","Portugal"} #
DATA.resetNext()
length=0
loop while DATA.hasNext()
    DATA.getNext()
    length+=1
end loop
CITY = array(length/2)
COUNTRY = array(length/2)
count = 0
DATA.resetNext()
loop while DATA.hasNext()
    CITY[count] = DATA.getNext()
    CAPITAL[count] = DATA.getNext()
    count += 1
end loop
```

**proof**
```.py
CITY = ["Ankara","Tokyo","Lisbon"]
CAPITAL = ["Turkey","Japan", "Portugal"]
```
![](https://github.com/marinamen/year2/blob/main/quizzes/media/IMG_E43BE7B6F754-1.jpeg)
