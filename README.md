# Simplified_Stock_Price_Simulation

This is highly simplified, it makes simplified assumptions e.g it does apply geometric brownian motion
It is NOT a perfect model simulation

### Libraries

- yFinance: To retrive stock prices
- Numpy: for calcuations and to generate random numbers
- Matplotlib: result visualisations 

The stock used is the tesla stock, only the adjusted closing price is stored in the datafreme. 


## Calculate Returns

Need the returns in order to define the paremetrs for the random function. To retieve daily reutnes
the pct_change() function is called, along with te log(), to normalise the results 

Random Function: Based on a normal distriubtion with the given parameters:
                 
   μ for the mean return of tesla 
   
   Sigma which retruns σ
   
## Get Simulated Prices

Taking the most recent price of tesla this is multplied with the simulated returns normal distrubtion.
Then take the cumulative product of that operation to get the gernated prices for Tesla for x years. 

## Visualisations


The Ren Walk of the tesla price of the next 252 trading days based on the random generated number in a normal distribution

![Ren Walk Image](https://github.com/EziOzoani/Simplified_Stock_Price_Simulation/blob/master/Images/Single%20Ren.png) 

Create multiple random walks 
Note: Black line is reference price

![Multi Ren Walk Image](https://github.com/EziOzoani/Simplified_Stock_Price_Simulation/blob/master/Images/Multi%20Ren.png)
   
