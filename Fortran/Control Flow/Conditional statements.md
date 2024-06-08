# Conditional statements
![[Rotation-If-Statments-in-After-Effects.gif]]

---

## কন্ডিশনাল স্টেটমেন্ট কি? 
প্রোগ্রামিংয়ে, কন্ডিশনাল  স্টেটমেন্ট হলো এমন একটি মৌলিক গঠন যা নির্দিষ্ট শর্তের উপর ভিত্তি করে আপনার প্রোগ্রামের কার্যক্রমের প্রবাহকে নিয়ন্ত্রণ করে। এটি আপনার প্রোগ্রামকে সিদ্ধান্ত নেওয়ার এবং কোনও শর্ত সত্য বা মিথ্যা তার উপর ভিত্তি করে বিভিন্ন কোড ব্লক চালানোর অনুমতি দেয়।

---

Fortran provides the following types of Conditional statements.

| Sr.No | Statement & Description       |
| ----- | ----------------------------- |
| 1     | ==If… then construct<br>==        |
| 2     | ==If… then...else construct==     |
| 3     | ==If...else if...else Statement== |
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
       
   print*, "Out of conditional Statement"
 end program ifProg
```


---


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
       
   print*, "Out of conditional Statement"
	
end program ifElseProg
```


---


## 3. Syntax of If ... Else ... If ... Else 

![[Pasted image 20240608145505.png|300]]

---

```
if (logical expression 1) then 
   ! block 1   
else if (logical expression 2) then       
   ! block 2   
else if (logical expression 3) then       
   ! block 3  
else       
   ! block 4   
end if
```

---
### Example 
```
program ifElseIfElseProg

   integer :: a = 100

   if( a == 10 ) then
      print*, "Value of a is 10" 


   else if( a == 20 ) then
      print*, "Value of a is 20" 


   else if( a == 30 ) then
      print*, "Value of a is 30" 
  
   else
      print*, "None of the values is matching" 
      
   end if
   
   print*, "Out of conditional Statement"
 
end program ifElseIfElseProg
```


