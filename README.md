# SQLTest

SELECT P.ProductName, ISNULL(C.CategoryName, 'Нет категории') AS CategoryName
FROM Products P
LEFT JOIN ProductCategory PC ON P.ProductID = PC.ProductID
LEFT JOIN Categories C ON PC.CategoryID = C.CategoryID;
