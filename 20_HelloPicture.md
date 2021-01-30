# HelloPicture



## Code

```python
print('Hi!')
```

    Hi!


## Picture

This is a PNG:
![company_logo.png](attachment:company_logo.png)

And this a JPG:
![Delphin.jpg](attachment:Delphin.jpg)

## a Plot

```python
import matplotlib as mpl

import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(0, 10, 500)
y = np.sin(x)

fig, ax = plt.subplots()

# Using set_dashes() to modify dashing of an existing line
line1, = ax.plot(x, y, label='Using set_dashes()')
line1.set_dashes([2, 2, 10, 2])  # 2pt line, 2pt break, 10pt line, 2pt break

# Using plot(..., dashes=...) to set the dashing when creating a line
line2, = ax.plot(x, y - 0.2, dashes=[6, 2], label='Using the dashes parameter')

ax.legend()
plt.show()
```


![png](20_HelloPicture_files/output_6_0.png)

