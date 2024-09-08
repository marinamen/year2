# quiz 075

```.py
import matplotlib.pyplot as plt
import numpy as np

def calculate_parity(n):
    k = 0
    while (2**k) < (n + k + 1):
        k += 1
    return k

def efficiency(lengths):
    efficiencies = []
    for l in lengths:
        parity = calculate_parity(l)
        total_bits = l + parity
        eff = l / total_bits
        efficiencies.append(eff)
    return efficiencies

lengths = np.arange(1, 1000)

efficiencies = efficiency(lengths)

plt.figure(figsize=(10, 6), facecolor='lightpink')
plt.plot(lengths, efficiencies, marker='*',color='pink')
plt.title('efficiency against length')
plt.xlabel('length( bits)')
plt.ylabel('efficiency ')
plt.grid(True)
plt.show()

```
![](https://github.com/marinamen/year2/blob/main/quizzes/media/Screenshot%202024-09-09%20at%2008.27.41.png)
