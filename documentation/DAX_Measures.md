\# DAX Measures



\## Total Sales



```DAX

Total Sales =

SUM(Orders\[SalesAmount])



Total Profit =

SUM(Orders\[Profit])



Total Orders =

DISTINCTCOUNT(Orders\[OrderID])



Total Customers =

DISTINCTCOUNT(Orders\[CustomerID])



Average Order Value =

DIVIDE(

&#x20;   \[Total Sales],

&#x20;   \[Total Orders],

&#x20;   0

)



Profit Margin % =

DIVIDE(

&#x20;   \[Total Profit],

&#x20;   \[Total Sales],

&#x20;   0

)



Returned Orders =

DISTINCTCOUNT(Returns\[OrderID])



Return Rate % =

DIVIDE(

&#x20;   \[Returned Orders],

&#x20;   \[Total Orders],

&#x20;   0

)



Previous Year Sales =

CALCULATE(

&#x20;   \[Total Sales],

&#x20;   SAMEPERIODLASTYEAR(DimDate\[Date])

)



YoY Growth % =

DIVIDE(

&#x20;   \[Total Sales] - \[Previous Year Sales],

&#x20;   \[Previous Year Sales],

&#x20;   0

)





