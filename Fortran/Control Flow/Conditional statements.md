Fortran provides the following types of decision making constructs.

| Sr.No | Statement & Description       |
| ----- | ----------------------------- |
| 1     | If… then construct<br>        |
| 2     | If… then...else construct     |
| 3     | If...else if...else Statement |
| 4     | Nested if construct           |
| 5     | Select case construct<br>     |
| 6     | Nested select case construct  |

---

## 1. Syntax of If .... Then

![[Pasted image 20240608143123.png]]
```
if (logical expression) then      
   statement  
end if
```

---
### Example 
```
program ifProg
   integer :: a = 10
 
   if (a < 20 ) then
   
   print*, "a is less than 20"
   end if
       
   print*, "No Condition"
 end program ifProg
```




## 2. Syntax of If ... Then ... Else 

![[Pasted image 20240608144546.png]]
```
if (logical expression) then      
   statement(s)  
else
   other_statement(s)
end if
```

---
### Example 
```
program ifElseProg
   integer :: a = 100
 
   if (a < 20 ) then
   print*, "a is less than 20"
   
   else
   print*, "a is not less than 20"
   
   end if
       
   print*, "value of a is "
	
end program ifElseProg
```
