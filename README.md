# spoisson

Sparse linear solver for 2d problems

# Installation

python setup.py install --user

# Usage

for the default poisson operator


```
import numpy as np
import spoisson

N = 100

x = np.linspace(0,1,N)
y = np.linspace(0,1,N)
xx,yy = np.meshgrid(x,y)

rhs = np.sin(2*np.pi*yy)

sol = spoisson.sol(rhs)
```

You can generalize `poisson2d` to any linear operator