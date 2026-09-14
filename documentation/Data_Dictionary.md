\# Data Dictionary



\## Customers



| Column | Description |

|---|---|

| CustomerID | Unique customer identifier |

| CustomerName | Customer name |

| Gender | Customer gender |

| Age | Customer age |

| City | Customer city |

| State | Customer state |

| Region | Customer region |

| CustomerSegment | Customer segment |



\## Products



| Column | Description |

|---|---|

| ProductID | Unique product identifier |

| ProductName | Product name |

| Category | Product category |

| SubCategory | Product sub-category |

| UnitPrice | Selling price per unit |

| CostPrice | Product cost |



\## Orders



| Column | Description |

|---|---|

| OrderID | Unique order identifier |

| OrderDate | Date of order |

| CustomerID | Customer reference |

| ProductID | Product reference |

| Quantity | Units ordered |

| Discount | Discount applied |

| SalesAmount | Revenue generated |

| Profit | Profit generated |

| Region | Order region |

| OrderStatus | Completed, Cancelled or Pending |



\## Returns



| Column | Description |

|---|---|

| ReturnID | Unique return identifier |

| OrderID | Related order |

| ReturnDate | Return date |

| ReturnReason | Reason for return |

| ReturnStatus | Return status |



\## Regions



| Column | Description |

|---|---|

| RegionID | Location identifier |

| Region | Geographic region |

| State | State |

| City | City |

