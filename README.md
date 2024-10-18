# Hairdresser Simulation
 Code for a makeshift hairdresser simulation that was outlined in one of my maths lectures

 The process goes as follows:
 Customer enters store
 Waits for a hairdresser to become available 
 Determines whether they want a haircut (10 minutes) or haircut and shampoo (20 minutes)
 Has the job performed and leaves

 The chance of a customer entering the store is dependent on the input value, and varies with time according to the equation (a * math.exp(-(((env.now/60) - 4) ** 2) / 10))
    Where a is a constant based off the input
    env.now/60 represents the current time in hours 

    This is to better reflect the customer intake across peak and non-peak hours
