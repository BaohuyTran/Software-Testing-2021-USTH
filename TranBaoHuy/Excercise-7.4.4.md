# Excercise 7.4.4
---

```Java
public static void trash (int x)    
{                         
   int m, n;                 

   m = 0;                    
   if (x > 0)               
      m = 4;                
   if (x > 5)              
      n = 3*m;              
   else                     
      n = 4*m;             
   int o = takeOut (m, n);
   System.out.println ("o is: " + o);  
}
public static int takeOut (int a, int b)
{
   int d, e;

   d = 42*a;
   if (a > 0)
      e = 2*b+d;
   else
      e = b+d;
   return (e);
}
```

### a)

For variable `m`, lines are 3, 5, 7, 9, 11, 12

For variable `n`, lines are 3, 9, 11, 12

### b)

For variable `m`, last def is in line 7, first use is in line 9

For variable `n`, last def is in line 11, first use is in line 21

### c)

x = 1; x = 6; x = 0