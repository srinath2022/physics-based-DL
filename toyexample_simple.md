---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(python_by_example)=

# A Toy Example

We will start off by considering a toy example of tossing a coin and eventually add air resistance etc. Let us begin by writing down the velocity and displacement equations of a point mass object thrown vertically above the ground with an initial velocity $u_0$.   

Under the effect of gravity, the velocity of the object at any time instant from start($t=0$) is given by   

$ v_t = u_0 + gt $   

where $g$ represents acceleration due to gravity $\sim 10 \frac{m}{s^2}$ 

Also, the displacement covered by the point mass is given by

$ s_t = u_0t + \frac{1}{2}gt^2 $

(whileloopprog)=

```{code-cell} python3
ts_length = 100
ϵ_values = []
i = 0
while i < ts_length:
    e = np.random.randn()
    ϵ_values.append(e)
    i = i + 1
plt.plot(ϵ_values)
plt.show()
```