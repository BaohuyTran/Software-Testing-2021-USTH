# Excercise 9.2.3
---

## Original

```Java
public static int sum(int[] x)
   {
      int s = 0;
      for (int i=0; i < x.length; i++)
      {
         s = s + x[i];
      }
      return s;
   }
```

## Mutant

```Java
public static int sum(int[] x)
   {
      int s = 0;
      for (int i=0; i < x.length; i++)
      {
         s = s - x[i];
      }
      return s;
   }
```

### a)

Impossible

### b)

Impossible

### c)

All zeros

### d)

All ones
