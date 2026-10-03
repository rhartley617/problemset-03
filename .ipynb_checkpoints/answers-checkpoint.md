# CMPS 6610 Problem Set 03
## Answers

**Name:<u>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rob Hartley</u>___________


Place all written answers from `problemset-03.md` here for easier grading.




- **1b.**  
$W(n) =W(n -1) +1$

    level 1  
  $W(n - 1) = 1 \cdot (W(n -1 -1) + 1) + 1$  
  $W(n - 1) = W(n -2) + 2$

  level 2  
  $W(n - 2) = 1 \cdot (W(n-2 - 1) + 1) + 2$  
  $W(n - 2) = W(n - 3) + 3$

  Generalized Equation  
    $W(n) = W(n - k) + k + 1$

  Recursion Depth  
  $n - k = 0$

  Substitute  
  $W(n) = W(n - n) + n$  
  $W(n) = W(0) + n$

  $\boxed{W(n) \in \Theta(n)}$

  $\boxed{S(n) \in \Theta(n)}$
  




- **1d.**  
  $W(n) = 2W(\frac{n}{2}$





- **1e.**





- **2a.**





- **2b.**





- **2c.**






- **3b.**





- **3d.**





- **3f.**




