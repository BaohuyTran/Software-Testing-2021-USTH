# Excercise-7.2.2.7
---

[The graph](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+3%0D%0A1+2%0D%0A2+3%0D%0A2+1%0D%0A3+1%0D%0A&initialNode=1&endNode=3&action=Nodes)

### a)

p5 is not a test path because it's impossible to reach 2 from 3 directly

### b)

|Test Paths|	Test requirements patrolled directly by the test path|
|---|---|
|[1,3,1,2,3]|	[1,3,1], [1,2,3], [3,1,2]|
|[1,2,1,2,3]|	[1,2,3], [1,2,1], [2,1,2]|
|[1,2,3,1,2,3]|	[1,2,3], [2,3,1], [3,1,2]|
|[1,2,1,3]|	[1,2,1], [2,1,3]|
|[1,2,3,1,3]|	[1,2,3], [2,3,1], [3,1,3]|

### c)

From b), p1, p4 don't satisfy

### d)

The answer is No.

With a sidetrip: [3, 1, 2, 1, 3]
