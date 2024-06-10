## Conditional statements Part-2
![[Rotation-If-Statments-in-After-Effects.gif]]

---
### Nested If Construct
You can use one **if** or **else if** statement inside another **if** or **else if** statement(s).

---

## Syntax

```
if ( logical_expression 1) then
   
   if(logical_expression 2)then 

   end if
end if

```

---

## Example
```
program nestedIfProg
implicit none

   integer :: a = 100, b= 200
 

   if( a == 100 ) then
      
	   if( b == 200 ) then
  
	   print*, "Value of a is 100 and b is 200" 
  
	   end if
   end if
   
   print*, "exact value of a is ", a
   print*, "exact value of b is ", b
 
end program nestedIfProg

```


---
### Select case construct
একটি **select case**  স্টেটমেন্ট কোনো ভেরিয়েবলকে (variable) মানগুলির একটি তালিকার বিপরীতে সমান কিনা তা পরীক্ষা করার অনুমতি দেয়। প্রতিটি মানকে একটি ক্ষেত্র (case) বলা হয়, এবং নির্বাচিত ভেরিয়েবলটি প্রতিটি নির্বাচন ক্ষেত্রের জন্য চেক করা হয়।
### Syntax

The syntax for the **select case** construct is as follows −

[name:] select case (expression) 
   case (selector1)          
   ! some statements          
   ... case (selector2)           
   ! other statements           
   ...       
   case default          
   ! more statements          
   ...   
end select [name]

The following rules apply to a **select** statement −

- The logical expression used in a select statement could be logical, character, or integer (but not real) expression.
    
- You can have any number of case statements within a select. Each case is followed by the value to be compared to and could be logical, character, or integer (but not real) expression and determines which statements are executed.
    
- The constant-expression for a case, must be the same data type as the variable in the select, and it must be a constant or a literal.
    
- When the variable being selected on, is equal to a case, the statements following that case will execute until the next case statement is reached.
    
- The case default block is executed if the expression in select case (expression) does not match any of the selectors.
    

### Flow Diagram

![Flow Diagram2](https://www.tutorialspoint.com/fortran/images/select_case_flow_diagram.jpg)

### Example 1

[Live Demo](http://tpcg.io/9sqOQB)

program selectCaseProg
implicit none

   ! local variable declaration
   character :: grade = 'B'

   select case (grade)
   
      case ('A') 
      print*, "Excellent!" 

      case ('B')
      
      case ('C') 
         print*, "Well done" 

      case ('D')
         print*, "You passed" 

      case ('F')
         print*, "Better try again" 

      case default
         print*, "Invalid grade" 
      
   end select
   
   print*, "Your grade is ", grade 
 
end program selectCaseProg

When the above code is compiled and executed, it produces the following result −