# CMPS 6610 Problem Set 03
## Answers

**Name:<u>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rob Hartley</u>___________


Place all written answers from `problemset-03.md` here for easier grading.




- **1b.**  
$W(n) =W(n -1) +1$

    Level 1  
  $W(n) = (W(n -1 -1) + 1) + 1$  
  $W(n) = W(n -2) + 2$

  Level 2  
  $W(n) = (W(n-2 - 1) + 1) + 2$  
  $W(n) = W(n - 3) + 3$

  Generalized Equation  
    $W(n) = W(n - k) + k$

  Recursion Depth  
  $n - k = 0$
  $k = n$

  Substitute  
  $W(n) = W(n - n) + n$  
  $W(n) = W(0) + n$

  $\boxed{W(n) \in \Theta(n)}$

  $\boxed{S(n) \in \Theta(n)}$
  




- **1d.**  
  $W(n) = 2W(\frac{n}{2}) + 1$  

  Level 1  
  $W(n) = 2 \cdot (2W(\frac{n}{4} + 1) + 1$  
  $W(n) = 4W(\frac{n}{4}) + 3$  

  Level 2  
  $W(n) = 4 \cdot (2W(\frac{n}{8} + 1) + 3$  
  $W(n) = 8W(\frac{n}{8}) + 7$  

  Generalized Equation    
  $W(n) = 2^kW(\frac{n}{2^k}) + (2^k - 1)$

  Recursion Depth    
  $\frac{n}{2^k} = 1$  
  $n = 2^k$   
  $k = \lg n$  

  Substitute  
  $W(n) = 2^{\lg n}W(\frac{n}{2^k}) + (2^{\lg n} - 1)$  
  $W(n) = nW(1) + n - 1$

  $\boxed{W(n) \in \Theta{n}}$

  $S(n) = S(\frac{n}{2}) + 1$

  Level 1  
  $S(n) = S(\frac{n}{4}) + 1 + 1$  
  $S(n) = S(\frac{n}{4}) + 2$

  Level 2  
  $S(n) = S(\frac{n}{8}) + 1 + 2$  
  $S(n) = S(\frac{n}{8}) + 3$

  Generalized Equation  
  $S(n) = S(\frac{n}{2^k}) + k$

  Recursion Depth  
  $\frac{n}{2^k} = 1$  
  $n = 2^k$  
  $k = \lg n$  

  Substitute  
  $S(n) = S(\frac{n}{2^{\lg n}}) + \lg n$  
  $S(n) = S(1) + \lg n$

  $\boxed{S(n) \in \Theta(\lg n)}$

  
  





- **1e.**





- **2a.**





- **2b.**





- **2c.**






- **3b.**





- **3d.**





- **3f.**




