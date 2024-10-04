## Stock Portfolio Assignment

**Rajsi Traders** is a small firm that has launched a platform where it will display a few stocks which is for working employees. In their platform, they have a few stocks mentioned which you can add to your portfolio and it will also generate the “Profit/Loss” scenario based on the market price and current stock price.

### **What is the Stock portfolio Platform?**

1.  The user can see 6 most relevant stocks on the platform.
    
2.  To move ahead, they need to add at least 4 stocks in their portfolio first.
    
3.  While adding the stocks, the user also needs to mention the quantity of the stocks they wish to purchase.
    
4.  Once added, it will generate the Market Price and Bought At price automatically.
    

Once you have added all the stocks, the user can see their “Stock Portfolio”

1.  When the user clicks “View Returns” for each stock, they will be able to see the return for each stock they have added in their portfolio. **Return = (marketPrice - boughtAt) * quantity**
    
2.  Now, the user will need to calculate the return percentage based on the returns they received which will be: **returnPercentage = (returns / boughtAt) * 100**
    
3.  After calculating the Return Percentage, the user can now see the “Status” of their stock portfolio for each stock Profit or Loss
    
4.  And at the end, the user can see their cumulative result of the portfolio
    
    1.  Total Returns
        
    2.  Total Growth

## API End Points:

### Endpoint 1: Calculate the Returns of the Stocks added
```
http://localhost:3000/calculate-returns?boughtAt=300&marketPrice=400&quantity=2
```
### Endpoint 2: Calculate the Total Returns
```
http://localhost:3000/total-returns?stock1=100&stock2=200&stock3=200&stock4=400
```
### Endpoint 3: Calculate the Return Percentage
```
http://localhost:3000/calculate-return-percentage?boughtAt=400&returns=200
```
### Endpoint 4: Calculate the Total Return Percentage
```
http://localhost:3000/total-return-percentage?stock1=10&stock2=20&stock3=20&stock4=40
```
### Endpoint 5: Identify the Status of Stocks based on their Return Value
```
http://localhost:3000/status?returnPercentage=90
```

  **Deployed Link:**  [Stock Portfolio Assignment](https://stock-portfolio-assignment.vercel.app/)
  
  **Note:** Check API endpoints on the deployed link or use this frontend application - [UI](https://bd1-stocks.vercel.app/) to API response.
