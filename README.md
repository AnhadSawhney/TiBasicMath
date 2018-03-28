# TiBasicMath
A collection of programs written in Ti-Basic to solve precalculus problems

# Programs:
### Lagrange: 
Calculates the unsimplified equation of a function using lagrange interpolation given any number of points.
Since the equations can get very long it prints each part on a separate line and prints the coefficients separately.
The full function is stored in str2.

Instructions:
1. Run the program.
2. Specify the number of points (length). Keep in mind a line is defined by 2 points a quadratic by 3, cubic by 4 etc.
3. Enter x coordinates of all points
4. Enter y coordinates of all points

### Simplify: 
Takes the output of the lagrange program (the function stored in str2) or user input and simplifies it.

*NOTE: Simplify is not capable of processing functions more complex than cubics.*

Instructions:
1. Run the program
2. Select user input or existing (lagrange) output
3. Enter user input if selected (See USER INPUT at bottom)

### Newsimpl: 
Takes the output of the lagrange program (the function stored in str2) or user input and simplifies it.

*NOTE: This program is not compatible with old firmware versions (ie. ones that dont have tostring(). This program can deal with functions up to the 5th degree (quintics).*

Instructions:
1. Run the program
2. Select user input or existing (lagrange) output
3. Enter user input if selected (See USER INPUT at bottom)

### Triangle: 
Given 3 measurements of a triangle with at least one side, (either 2 sides + one angle, 2 angles + one side or 3 sides),
calculates the other 3 measurements along with the area and radius of the inscribed circle. Will calculate both cases of SSA.
(Uses law of sines/cosines and heron's formula)

*NOTE: Calculator and angles must be in degree mode.*

Instructions:
1. Run the program
2. Enter angles. (Enter 0 if you want the calculator to find the value)
3. Enter sides. (Enter 0 if you want the calculator to find the value)

### Sinusoid: 
Given the coordinates of two adjacent peaks, find the equation of the sinusoid function (in the form f(x)=Asin(B(X+C))+D), with both sin and cos. 

Instructions:
1. Run the program
2. Enter x-coordinate of peak 1
3. Enter y-coordinate of peak 1
4. Enter x-coordinate of peak 2
5. Enter y-coordinate of peak 2

# Installation:
To install these programs, you need a usb cable to connect your calculator to a computer and the Ti-Connect software,
found here: https://education.ti.com/en/software/details/en/B59F6C83468C4574ABFEE93D2BC3F807/swticonnectsoftware

For Ti-84+ce calculators download ti connect ce.

These programs are formatted to work with Ti-84+ce calculators, currently the latest model. 
For best results use the latest version of the firmware which can be installed through ti connect as well.

### To transfer these programs to your calculator:
1. download the zip file and extract it anywhere on your computer.
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
4. Press `enter` to run it

### To exit the programs at any time press 2nd and mode (quit).
If you cannot exit by doing that it is probably waiting for you to press enter so press enter and then retry.

These programs will be erased if the ram on the calculator is reset. To prevent this you can archive them. If you do this they must be unarchived again in order to be run.

### To archive/unarchive programs on the calculator:
1. Press `2nd`
2. Press `mem` (plus)
3. Select `Mem management` (2)
3. Select `prgm` (7)
4. Move the cursor to the program. If it has a `*` before it it is archived. Press `enter` to archive/unarchive the selected program.

# USER INPUT FOR SIMPLIFY AND NEWSIMPL: 
Format must be `(X-@)(X-@)(X-@)...(X-@)*@+(X-@)(X-@)(X-@)...(X-@)*@`
### Terminology: 
`(X-@)(X-@)(X-@)...(X-@)*@` is a word
`(X-@)` is a letter

Each letter is in the format `(X-@)` where `@` is a real number. Everything except `@` must remain constant in all the letters.
If you want to do X+something then make it `(X--@)`. The letters are not separated from each other with anything.

Several letters strung together is a word. All words must have the same number of letters. 
The words must end with a coefficient in the form `*@` where `@` is a real number. 
If you do not want to multiply the word by anything end it with `*1`. Words are strung together with `+` and the values of `@`'s
in each letter can vary from word to word as well as the coefficient.

### Examples of valid user input:
`(X-1)(X-2)(X-3)*2+(X-4)(x-67)(x-12)*123`

`(X-1)*1`

`(X-0.5)(X-1.12)(X--4)*-12.75+(X-2.1)(X--3)(X--1.09)*3`
