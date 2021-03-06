It is customary to use matplotlib imshow to display the contents 
of a 2d matrix on a graphical way, but for small matrices (say smaller
than 10x10 or so) it might make sense to display the heatmap while printing
the numeric values of the pixels in the array.

Say we have a 3x3 numpy array of random values.

```
import numpy as np
values = np.random.uniform(low=0, high=10, size=[3,3])
```

Now lets display it with seaborn heatmap.

```
import matplotlib.pyplot as plt
import seaborn as sns

sns.heatmap(valuse, annot=True)
plt.show()
```

The image outputted will look like:

![Numerical values plot](/assets/images/2019-04-14-heatmap.png)
