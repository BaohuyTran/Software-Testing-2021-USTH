# Excercise 7.2.3.1
---


## a)

### Graph 1

[Link](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+2%0D%0A2+3%0D%0A2+8%0D%0A3+4%0D%0A3+5%0D%0A4+3%0D%0A5+6%0D%0A5+7%0D%0A6+7%0D%0A7+2%0D%0A&initialNode=1&endNode=8&action=Nodes)

### Graph 2

[Link](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+2%0D%0A2+3%0D%0A2+6%0D%0A3+4%0D%0A3+5%0D%0A4+5%0D%0A5+3%0D%0A&initialNode=1&endNode=6&action=Nodes)

### Graph 3

[Link](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+2%0D%0A2+3%0D%0A3+4%0D%0A3+5%0D%0A4+5%0D%0A5+2%0D%0A2+6%0D%0A&initialNode=1&endNode=&action=Nodes)

### Graph 4

[Link](https://cs.gmu.edu:8443/offutt/coverage/GraphCoverage?edges=1+2%0D%0A2+3%0D%0A2+6%0D%0A3+4%0D%0A3+5%0D%0A4+5%0D%0A&initialNode=1&endNode=6&action=Nodes)

## b)

dup1 [1, 2, 8]

dup2 [1, 2, 3, 5, 6]

dup3 [4, 3, 5, 6]

dup4 [4, 3, 5, 7, 2, 8]

dup5 [4, 3, 5, 6, 7, 2, 8]

## c)

||direct|with sidetrip|
|---|---|---|
|t1|dup1||
|t2||dup1|
|t3|dup2|dup1|
|t4|dup4||
|t5|dup3, dup5||
|t6||dup3, dup4, dup5|

## d)

dup1 (for def(1)), dup4 (for def(4))

## e)

dup1, dup3, dup5

## f)

dup1, dup3, dup4, dup5

