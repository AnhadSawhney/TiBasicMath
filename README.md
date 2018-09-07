# TiBasicMath
A collection of programs written in Ti-Basic to solve precalculus problems. Most of these programs are relevant to the Math 3 course.

## Introduction:
These programs are written and formatted for 3 different calculators: The Ti 84+ and the Ti 84+ ce / Ti 84+ c silver edition. Only used the files in the proper folder otherwise the text will be cut off. It is reccomended to use the latest firmware version when running these programs, although some of them will work without it.

If you are using a ti 84 plus calculator beware errors and formatting issues. I do not own this calculator model and cannot test the programs.

*NOTE: NEGATIVE NUMBERS IN ALL USER INPUT ARE ENTERED USING THE NEGATIVE NUMBER SIGN POSITIONED AT THE BOTTOM RIGHT OF THE KEYPAD.*
*READ THE ENTIRE README SO YOU ARE FAMILIAR WITH THE CAPABILITIES AND LIMITATIONS OF THESE PROGRAMS AND CAN USE THEM EFFECTIVELY.*
*IT IS HIGHLY RECCOMENDED TO UPDATE THE DEVICE OS BEFORE USING THESE PROGRAMS*

# Installation and Memory Management

To install these programs, you need a usb cable to connect your calculator to a computer and the Ti-Connect software,
found here: https://education.ti.com/en/software/details/en/CA9C74CAD02440A69FDC7189D7E1B6C2/swticonnectcesoftware

All of the three calculators mentioned above use the ti connect ce software. Install the version of the software that is made for your operating system (windows/osx/linux).

### To update the calculator OS

To update the calculator's operating system, visit this webpage https://education.ti.com/software/, select your calculator and download the os and apps bundle if availible, otherwise just the os. Then, connect the calculator to your computer with the USB cable and click Actions -> Send OS/Bundle to calculator. Finally, select the file you downloaded and wait for the installation to complete.

### To transfer these programs to your calculator:
1. Click "clone or download" at the top right corner, then click download zip
2. Extract the zip archive (Windows: right click and select extract all, Osx: double click)
2. Then open Ti connect and plug in your calculator with the usb cable.
3. Click on calculator explorer on the left side.
4. At the top should be a series of icons, select the one that looks like a laptop with an arrow pointing out.
5. Navigate to the folder you downloaded and select the program you want to send.
6. Click open. It should pull up a dialog box. 
7. Usually the default values are correct but just in case the name should be the same as the filename (without .8xp) and the location should be RAM. 
8. If you have multiple calculators connected select the one you want.
9. Check replace existing content with the same name if you are upgrading a program.
10. Press send and repeat the process with the other programs.

### To launch the programs from the calculator:
1. Press `prgm`
2. Select the program
3. Press `enter`. It should put you back on the default screen
4. Press `enter` again to run it

### To exit the programs at any time press `2nd` and `mode` (quit).
If you cannot exit by doing that it is probably waiting for you to press enter so press enter and then retry.

### To archive/unarchive programs on the calculator:
*NOTE: These programs will be erased if the RAM on the calculator is reset. To prevent this you can archive them. If you do this they must be unarchived again in order to be run.*
1. Press `2nd`
2. Press `mem` (plus)
3. Select `Mem management` (2)
3. Select `prgm` (7)
4. Move the cursor to the program. If it has a `*` before it it is archived. Press `enter` to archive/unarchive the selected program.

# Programs:
### Growth
This program is not intended for use in math, rather Biology. It will calculate the equations for the logistic and exponential population growth models.

Instructions:
1. Run the program
2. Choose Exponential or Logistic growth by entering 1 or 2
3. Enter the required information
4. The output function will be stored in the `y=` menu

### Lagrange
Calculates the unsimplified equation of a function using lagrange interpolation given any number of points.
Since the equations can get very long it prints each part on a separate line and prints the coefficients separately.
The full function is stored in `str2`.

Instructions:
1. Run the program.
2. Specify the number of points (length). Keep in mind a line is defined by 2 points a quadratic by 3, cubic by 4 etc.
3. Enter x coordinates of all points
4. Enter y coordinates of all points

### Simplify
Takes the output of the lagrange program (the function stored in `str2`) or user input and simplifies it.

*NOTE: Simplify is not capable of processing functions more complex than cubics.*

Instructions:
1. Run the program
2. Select user input or existing output (only choose existing output if you have just run the lagrange program)
3. Enter user input if selected (See USER INPUT at bottom)
4. The output function will be stored in the `y=` menu

### Newsimpl
Takes the output of the lagrange program (the function stored in `str2`) or user input and simplifies it.

*NOTE: This program is not compatible with old firmware versions (ie. ones that dont have `tostring(`. This program can deal with functions up to the 5th degree (quintics)).*

Instructions:
1. Run the program
2. Select user input or existing output (only choose existing output if you have just run the lagrange program)
3. Enter user input if selected (See USER INPUT at bottom)
4. The output function will be stored in the `y=` menu

### Triangle
Given 3 measurements of a triangle with at least one side, (either 2 sides + one angle, 2 angles + one side or 3 sides),
calculates the other 3 measurements along with the area and radius of the inscribed circle. Will calculate both cases of SSA.
(Uses law of sines/cosines and heron's formula)
If all sides and angles are entered the calculator will perform a series of tests to see if the triangle is valid. 
(Ex: angles sum to 180)

*NOTE: Calculator must be in degree mode. For ti 84 plus ce calculators the mode is changed automatically*

Instructions:
1. Run the program
2. Enter angles. (Enter `0` if you want the calculator to find the value)
3. Enter sides. (Enter `0` if you want the calculator to find the value)

### Sinusoid
Given the coordinates of two adjacent peaks, find the equation of the sinusoid function (in the form `f(x)=Asin(B(X+C))+D)`), with both sin and cos. 

*NOTE: Calculator must be in radian mode. For ti 84 plus ce calculators the mode is changed automatically*

Instructions:
1. Run the program
2. Enter x-coordinate of peak 1
3. Enter y-coordinate of peak 1
4. Enter x-coordinate of peak 2
5. Enter y-coordinate of peak 2

### Invest
Given all but one of the following: principal (starting amount), years invested, annual percentage rate, number of times compounded per year, and ending value, find the missing value. 

*NOTE: Only one value can be marked as unknown.*

Instructions:
1. Run the program
2. Enter principal (Enter 0 if this value is unknown and you want the calculator to find it)
3. Enter years (Enter 0 if this value is unknown and you want the calculator to find it)
4. Enter annual percentage rate (Enter 0 if this value is unknown and you want the calculator to find it. Enter the entire rate without the perentage sign. Ex: for 9.75% enter 9.75)
5. Enter number of times compounded per year. (Enter 0 if this value is unknown and you want the calculator to find it. Enter -1 if the compounding is continuous.)
6. Enter ending value (Enter 0 if this value is unknown and you want the calculator to find it)

# User Input Formatting for SIMPLIFY and NEWSIMPL: 
Format must be `(X-@)(X-@)(X-@)...(X-@)*@+...+(X-@)(X-@)(X-@)...(X-@)*@`
### Info: 
`(X-@)(X-@)(X-@)...(X-@)*@` is referred to as a word

`(X-@)` is referred to as a letter

`@` is any real number. Replace this with a number when entering it in

### Rules:
Each letter is in the format `(X-@)` where `@` is a real number. Everything except `@` must remain constant in all the letters.
If you want to do X+something then make it `(X--@)`. The letters are not separated from each other with anything.

*NOTE: The second minus sign is not the operation minus. It is the negative number sign positioned at the bottom of the keypad.*

Several letters strung together is a word. All words must have the same number of letters. 
The words must end with a coefficient in the form `*@` where `@` is a real number. 
If you do not want to multiply the word by anything end it with `*1`. Words are strung together with `+` and the values of `@`'s
in each letter can vary from word to word as well as the coefficient.

*NOTE: The minus sign in the coefficient is not the operation minus. It is the negative number sign positioned at the bottom of the keypad.*

### Examples of valid user input:
`(X-1)(X-2)(X-3)*2+(X-4)(X-67)(X-12)*123`

`(X-1)*1`

`(X-0.5)(X-1.12)(X--4)*-12.75+(X-2.1)(X--3)(X--1.09)*3`
