# Excercise 8.2.1
---

## i)

f = ab(-c) + (-a)b(-c)

### a)

Karnaugh map for f

|c\a, b|00|01|11|10|
|---|---|---|---|---|
|0||1|1||
|1|||||

Karnaugh map for -f

|c\a, b|00|01|11|10|
|---|---|---|---|---|
|0|1|||1|
|1|1|1|1|1|

### b)

f = b(-c)

-f = (-b) + c

### c)

Answer in b)


### d)

```
Test Data:  
10 - UTP for term b!c  
MUTP is feasible for all terms.  
Number of tests: 1  

Number and types of mutants generated:  
Number of False mutants generated: 1  
Number of True mutants generated: 0  
Number of TOF mutants generated: 0  
Number of TIF mutants generated: 0  
Number of TRF mutants generated: 0  
Total Number of Non-Equivalent Mutants Generated: 1  

Mutants:  
(false)
```

### e)

```
Test Data:  
10 - UTP for term b!c  
00 - NFP for literal b in term b!c  
11 - NFP for literal c in term b!c  
CUTPNFP is feasible for all literals.  
Number of tests: 3  

Number and types of mutants generated:  
Number of False mutants generated: 1  
Number of True mutants generated: 0  
Number of TOF mutants generated: 0  
Number of TIF mutants generated: 2  
Number of TRF mutants generated: 0  
Total Number of Non-Equivalent Mutants Generated: 3  

Mutants:  
(false)  
b & !c | !b & !c  
b & !c | b & c
```

### f)

```
Test Data:  
00 - NFP for literal b in term b!c  
11 - NFP for literal c in term b!c  
MNFP is feasible for all literals.  
Number of tests: 2  

Number and types of mutants generated:  
Number of False mutants generated: 0  
Number of True mutants generated: 0  
Number of TOF mutants generated: 0  
Number of TIF mutants generated: 2  
Number of TRF mutants generated: 0  
Total Number of Non-Equivalent Mutants Generated: 2  

Mutants:  
b & !c | !b & !c  
b & !c | b & c  
```

## ii)

f = (-a)(-b)(-c)(-d) + abcd

## iii)

f = ab + a(-b)c + (-a)(-b)c

## iv)

f = (-a)(-b)(-d) + (-c)d + bcd
