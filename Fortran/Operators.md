**একটি অপারেটর হলো এমন একটি প্রতীক যা কম্পাইলারকে নির্দিষ্ট গাণিতিক বা লজিক্যাল ম্যানিপুলেশন সম্পাদন করার নির্দেশ দেয়। ফোরট্রান নিম্নলিখিত ধরনের অপারেটরগুলো সরবরাহ করে −**

- **গাণিতিক অপারেটর** (Arithmetic Operators)
- **সম্পর্কসূচক অপারেটর** (Relational Operators)
- **লজিক্যাল অপারেটর** (Logical Operators)

আসুন, আমরা এই সকল ধরনের অপারেটরগুলোকে এক এক করে দেখি।"


## Arithmetic Operators
নিম্নের টেবিলটি ফোরট্রানে সমর্থিত সকল গাণিতিক অপারেটরগুলো দেখায়। ধরে নেওয়া হলো ভেরিয়েবল A এর মান ৫ এবং ভেরিয়েবল B এর মান ৩।

| Operator | Description                                                            | Example              |
| -------- | ---------------------------------------------------------------------- | -------------------- |
| +        | Addition Operator, adds two operands.                                  | A + B will give 8    |
| -        | Subtraction Operator, subtracts second operand from the first.         | A - B will give 2    |
| *        | Multiplication Operator, multiplies both operands.                     | A * B will give 15   |
| /        | Division Operator, divides numerator by de-numerator.                  | A / B will give 1    |
| **       | Exponentiation Operator, raises one operand to the power of the other. | A ** B will give 125 |

## Relational Operators

নিম্নের টেবিলটি ফোরট্রানে সমর্থিত সকল সম্পর্কসূচক অপারেটরগুলো দেখায়। ধরে নেওয়া হলো ভেরিয়েবল A এর মান ১০ এবং ভেরিয়েবল B এর মান ২০, তাহলে −

|Operator|Equivalent|Description|Example|
|---|---|---|---|
|==|.eq.|Checks if the values of two operands are equal or not, if yes then condition becomes true.|(A == B) is not true.|
|/=|.ne.|Checks if the values of two operands are equal or not, if values are not equal then condition becomes true.|(A != B) is true.|
|>|.gt.|Checks if the value of left operand is greater than the value of right operand, if yes then condition becomes true.|(A > B) is not true.|
|<|.lt.|Checks if the value of left operand is less than the value of right operand, if yes then condition becomes true.|(A < B) is true.|
|>=|.ge.|Checks if the value of left operand is greater than or equal to the value of right operand, if yes then condition becomes true.|(A >= B) is not true.|
|<=|.le.|Checks if the value of left operand is less than or equal to the value of right operand, if yes then condition becomes true.|(A <= B) is true.|


## Logical Operators

ফোরট্রানে লজিক্যাল অপারেটরগুলো কেবলমাত্র লজিক্যাল মান .true. এবং .false. এর উপর কাজ করে।

নিম্নলিখিত টেবিলটি ফোরট্রানে সমর্থিত সকল লজিক্যাল অপারেটর দেখায়। ধরে নেওয়া হলো ভেরিয়েবল A এর মান .true. এবং ভেরিয়েবল B এর মান .false. , তাহলে −

| Operator | Description                                                                                                                                      | Example               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- |
| .and.    | Called Logical AND operator. If both the operands are non-zero, then condition becomes true.                                                     | (A .and. B) is false. |
| .or.     | Called Logical OR Operator. If any of the two operands is non-zero, then condition becomes true.                                                 | (A .or. B) is true.   |
| .not.    | Called Logical NOT Operator. Use to reverses the logical state of its operand. If a condition is true then Logical NOT operator will make false. | !(A .and. B) is true. |
| .eqv.    | Called Logical EQUIVALENT Operator. Used to check equivalence of two logical values.                                                             | (A .eqv. B) is false. |
| .neqv.   | Called Logical NON-EQUIVALENT Operator. Used to check non-equivalence of two logical values.                                                     | (A .neqv. B) is true. |



Source : https://www.tutorialspoint.com/fortran/fortran_operators.html