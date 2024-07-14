import matplotlib.pyplot as plt
import numpy as np 
def quadratic_temp_mode1(time):
  a=0.02
  b=1.5
  c=20
  temp=a* (time**2) + b * time + c
  return temp
time_values=np.arange(0,51,1)
temp_values=quadratic_temp_mode1(time_values)

plt.plot(time_values,temp_values,label='Temperature Model')
plt.xlabel('Time')
plt.ylabel('Temperature')
plt.title('Quadratic Temperature model')
plt.legend()
plt.grid(True)
plt.show()
