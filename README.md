# calculateSQRT

the effective way to calculate
$$
\sqrt{x^2 + y^2}
$$
don't worry can't calculate large integer. 

can't be overflow

- when we use $\sqrt{x^2+y^2}$ , we should calculate $x^2$ and $y^2$ first, it may cause the square of an integer can be overflow. 

### below is simple introduction for this solution.



1. calculate the ``maximum`` and ``minimum`` value of two number.

2. let R = $\frac{min}{max}​$ .

3. then `return `  $max \sqrt{1+R^2}​$ .

   

but we also can return $min \sqrt{1+R^2}$ , in this case R = $\frac{max}{min}$ .

you also can find this is not good as the first one.