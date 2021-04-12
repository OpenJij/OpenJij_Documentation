# Higher order model

If you want to handle higher order model as follows:

 ```math
 H = \sum_{i}h_i\sigma_i + \sum_{i < j} J_{ij} \sigma_i \sigma_j + \sum_{i, j, k} K_{i,j,k} \sigma_i\sigma_j \sigma_k \cdots
 ```

use ``.sample_hubo``

> HUBO: Higher order unconstraint binary optimization

## Sample code
```python
import openjij as oj

# Only SASampler can handle HUBO.
sampler = oj.SASampler()

# make HUBO
J = {(0,): -1, (0,1): -1, (0,1,2): 1}

response = sampler.sample_hubo(J, var_type="SPIN")
print(response)
#    0  1  2 energy num_oc.
# 0 +1 +1 -1   -3.0       1
# ['SPIN', 1 rows, 1 samples, 3 variables]

response = sampler.sample_hubo(J, var_type="BINARY")
print(response)
#    0  1  2 energy num_oc.
# 0  1  1  0   -2.0       1
# ['BINARY', 1 rows, 1 samples, 3 variables]
```
