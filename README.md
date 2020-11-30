# newtonRhapson
def f(x):
  return x**3 - 5*x - 9
def f_(x):
  return 3*x**2 - 5

x=0
step=0
cond=True

while (cond):
  h=(f(x)/f_(x))
  x=x-h
  step=step+1
  print(f' step {step} update {h}  root {x} ')
  
  cond=abs(h)>0.01


