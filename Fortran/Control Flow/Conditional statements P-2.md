## Conditional statements Part-2
![[Rotation-If-Statments-in-After-Effects.gif]]

---
### 4.Nested If Construct
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
### 5.Select case construct
একটি **select case**  স্টেটমেন্ট কোনো ভেরিয়েবলকে (variable) মানগুলির একটি তালিকার বিপরীতে সমান কিনা তা পরীক্ষা করার অনুমতি দেয়। প্রতিটি মানকে একটি ক্ষেত্র (case) বলা হয়, এবং নির্বাচিত ভেরিয়েবলটি প্রতিটি নির্বাচন ক্ষেত্রের জন্য চেক করা হয়।

---

### Syntax

```
select case (expression) 

	case (selector1)   
		!Something if True       
	case (selector2)      
		!Something if True     
	case default          
		!Something if True
  
end select 
```

---

### Flow Diagram

![Flow Diagram2](https://www.tutorialspoint.com/fortran/images/select_case_flow_diagram.jpg)

---

### Example 1

```
program selectCaseProg
implicit none

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
   
   ```
---
## 6.Nested select case construct

You can use one **select case** statement inside another **select case** statement(s).

---
## Syntax
```
select case(a) 

   case (100) 
      print*, "This is part of outer switch", a 

   select case(b) 
      case (200)
         print*, "This is part of inner switch", a 

   end select
      
end select
```


---

## Example

```
program nestedSelectCase
   integer :: a = 100
   integer :: b = 200
 
   select case(a) 
      case (100) 
         print*, "This is part of outer switch", a 
         
      select case(b) 
         case (200)
            print*, "This is part of inner switch", a 
      end select
      
   end select
   
   print*, "Exact value of a is : ", a 
   print*, "Exact value of b is : ", b 
 
end program nestedSelectCase
```
