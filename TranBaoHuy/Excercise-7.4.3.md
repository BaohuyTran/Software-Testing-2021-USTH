# Excercise 7.4.3
---

### a)

[The graph](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+2%0D%0A1+3%0D%0A2+3%0D%0A3+4%0D%0A3+5%0D%0A4+6%0D%0A5+6%0D%0A&initialNode=1+2+3+4+5+6&endNode=6&action=Nodes)

### b)

t1: [f1, f3, f5, f6]
t2: [f1, f3, f4, f6]
t3: [f1, f2]
t4: [f1, f3, f4, f6]
t5: [f1, f2, f3, f4, f6]

### c)

[3,5,6]
[1,2,3,4,6]

-> {t1, t2, t3}, {t1, t3, t4}, or {t1, t5}

### d)

[3,5,6]
[1,3,4,6]
[1,2,3,4,6]

-> {t1, t5}

### e)

- TR Prime path:
[1,2,3,4,6]
[1,2,3,5,6]
[1,3,4,6]
[1,3,5,6]

This one [1,2,3,5,6]