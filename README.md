# Monte Carlo Pi Estimation

A Python project to estimate the value of π (pi) using the Monte Carlo method.  
Includes interactive visualization of the simulation and the convergence of the estimate.

---

## Features

- Generate random points inside a unit square.
- Check if points fall inside a circle centered at (0.5, 0.5) with radius 0.5.
- Calculate the π estimate based on the ratio of points inside the circle.
- Plot the points inside and outside the circle with matplotlib.
- Show convergence of the estimate to the real π value as the number of points increases.
- Interactive slider widget to dynamically change the number of points used in the simulation.

---

## Requirements

- Python 3.7+
- numpy
- matplotlib
- ipywidgets (for the interactive slider in Jupyter notebooks)

Install dependencies using pip:

```bash
pip install numpy matplotlib ipywidgets
```

## How it works

The Monte Carlo method estimates π by:

1. Randomly sampling points in the square ![White formula](https://latex.codecogs.com/png.latex?\color{white}{[0,1]%20\times%20[0,1]}).
2. Counting how many points fall inside the circle of radius 0.5 centered at (0.5, 0.5).
3. Using the ratio of points inside the circle to the total points to approximate π as:

![Pi formula in white](https://latex.codecogs.com/png.latex?\color{white}{\pi%20\approx%204%20\times%20\frac{\text{Number%20of%20points%20inside%20circle}}{\text{Total%20number%20of%20points}}})
