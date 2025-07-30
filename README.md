# Power-BI-practice

1. Product
plaintext
Copy
Edit
- ProductKey (Primary Key)
- Product
- Category
- Subcategory
- Color
- Standard Cost
2. Region
plaintext
Copy
Edit
- SalesTerritoryKey (Primary Key)
- Country
- Group
- Region
3. Reseller
plaintext
Copy
Edit
- ResellerKey (Primary Key)
- Reseller
- Business Type
- City
- Country-Region
- State-Province
4. Salesperson
plaintext
Copy
Edit
- EmployeeKey (Primary Key)
- EmployeeID
- Salesperson
- Title
- UPN
5. Targets
plaintext
Copy
Edit
- EmployeeID (Foreign Key to Salesperson.EmployeeID)
- Target
- TargetMonth
6. Sales
plaintext
Copy
Edit
- ProductKey (Foreign Key to Product.ProductKey)
- EmployeeKey (Foreign Key to Salesperson.EmployeeKey)
- OrderDate
- Quantity
- Cost
7. SalespersonRegion
plaintext
Copy
Edit
- EmployeeKey (Foreign Key to Salesperson.EmployeeKey)
- SalesTerritoryKey (Foreign Key to Region.SalesTerritoryKey)
🔗 Relationships (Diagram Arrows Summary)
Sales.ProductKey → Product.ProductKey (Many-to-One)

Sales.EmployeeKey → Salesperson.EmployeeKey (Many-to-One)

Targets.EmployeeID → Salesperson.EmployeeID (Many-to-One)

SalespersonRegion.EmployeeKey → Salesperson.EmployeeKey (Many-to-One)

SalespersonRegion.SalesTerritoryKey → Region.SalesTerritoryKey (Many-to-One)

Reseller.SalesTerritoryKey → Region.SalesTerritoryKey (Many-to-One)
