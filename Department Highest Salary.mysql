Select Department.Name as Department, emp1.Name as Employee, emp1.Salary 
from Employee emp1 join Department on emp1.DepartmentId = Department.Id
where emp1.Salary = (Select Max(Salary) from Employee emp2 where emp2.DepartmentId = emp1.DepartmentId);
