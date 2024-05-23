he Fortran output system allows you to display data and messages to the user or write them to external files. Here's a breakdown of the key concepts:

**1. Unformatted vs. Formatted Output:**

- **Unformatted Output (WRITE statements):**
    - Used for simple data printing without specific formatting.
    - You specify the variables or expressions to be written, separated by commas.
    - Example: `WRITE(*,*) x, y, z` (prints variables x, y, and z)
- **Formatted Output (PRINT statements):**
    - Offers more control over how data is displayed.
    - Uses a format specifier to define the layout of the output.
    - Example: `PRINT *, 'Result:', F10.2` (prints "Result:" followed by a floating-point number with 2 decimal places)

**2. Format Specifiers:**

- Format specifiers control how data is displayed in formatted output (PRINT statements).
- They define:
    - Data type (integer, real, character, etc.)
    - Field width (minimum number of characters to display)
    - Precision (number of decimal places for floating-point numbers)
    - Other formatting options like justification (left, right, or center)
- Common format specifiers:
    - `I` - Integer
    - `F` - Floating-point
    - `E` - Scientific notation
    - `A` - Character string

**3. Output Unit Control:**

- By default, unformatted output (`WRITE`) goes to the console.
- Formatted output (`PRINT`) can be directed to different output units:
    - `*` - Console (default)
    - Unit number (associated with an external file opened with `OPEN` statement)
- This allows you to write output to specific files for further processing or analysis.

**4. Error Handling:**

- It's essential to handle potential errors during output operations.
- Fortran provides features to check for errors like file I/O errors or invalid format specifiers.
- You can use statements like `ERRNO` and `IOSTAT` to detect and handle errors gracefully.

**Here's an example illustrating both unformatted and formatted output:**

Fortran

```
program output_example
  integer :: age = 25
  real :: pi = 3.14159
  character(len=10) :: name = "Fortran"

  ! Unformatted output
  write(*,*) "Name:", name, " Age:", age

  ! Formatted output
  print *, "Pi with 4 decimals:", F10.4
  print *, 'Formatted string: ', A

end program
```

Use code [with caution.](/faq#coding)

content_copy

This code will print something like:

```
Name: Fortran  Age: 25
Pi with 4 decimals:    3.1416
Formatted string: Fortran
```

**In summary, the Fortran output system provides flexibility for displaying data in various ways, allowing you to tailor the output to your specific needs.**