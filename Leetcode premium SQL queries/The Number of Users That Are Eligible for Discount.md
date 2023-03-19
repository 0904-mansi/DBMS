![Screenshot from 2023-03-19 20-39-54](https://user-images.githubusercontent.com/81081105/226185639-6e97a156-42f9-4237-9341-aa869ea0f75a.png)

# using function

```sql
# Time:  O(n)
# Space: O(n)

CREATE FUNCTION getUserIDs(startDate DATE, endDate DATE, minAmount INT) RETURNS INT
BEGIN
  RETURN (
    SELECT COUNT(DISTINCT user_id) AS user_cnt
    FROM Purchases
    WHERE time_stamp >= startDate AND time_stamp <= endDate AND amount >= minAmount
  );
END

```


# using procedure

```sql

CREATE PROCEDURE getUserIDs (startDate DATE,
endDate DATE, minAmount INT)
BEGIN

# Write your MySQL query statement below.
SELECT DISTINCT user_id
FROM Purchases
WHERE time stamp BETWEEN startDate AND endDate
AND amount >= minAmount

END
```
