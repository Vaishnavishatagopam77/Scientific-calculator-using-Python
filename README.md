# Scientific-calculator-using-Python

# Introduction:
In this project, we build up the scientific calculator using the tkinter library of Python. It is the standard GUI library for Python. With its help, we prepared the GUI for the project, and to add the functionalities of the scientific calculator, we used a math module. So, scroll down and get to know the steps!

# Explanation:
The first step is importing all the necessary libraries using the “import” keyword. For the latest version, the tkinter module comes under the future module. So first, we have to install the future module with the help of the command “pip install <module-name>”. The future module is a built-in module in Python that inherits new features which is available in the latest Python versions. With “future. moves” we will import the tkinter module.

In the next step, to create an object of the tkinter frame will use “.Tk()”.With this, we will also set the title and geometry of our tkinter application. To set the background color for the project we will use “.config(bg=<color name>)”. And so, with that, we have set black as the background color for this project.

We will also add an image by the corner to give it a creative aspect. With the help of “.PhotoImage(file=<filename>)”, we will load the picture, by using the “.Label()” we will make the label widget for this, and “.grid(row=,column= )” will help to get it placed well on the window.

While working on this project, we need to fulfill three aspects.

Space for the calculation
Buttons for the calculation
Adding the functionalities
Talking about the first aspect, we will create an entry widget by “.Entry()”. Under this, we have provided the parameter such as

root – window object

font – The font style in which we want the information to get entered

bg – Stating the background color for the space

fg – Stating the color of the text appeared

bd – Border of the entry widget

width – width of the entry widget

Finally, with the help of “.grid()” we will set the position for the entry widget.

Getting into the next aspect, first of all, we have to create a list containing all the buttons that need to appear on the calculator. In this list, we will represent some characters by encoding them. Since the “.grid()” function works with row and column parameters. Therefore, we will take two variables for the same and then we run a “for” loop for creating the buttons by “.Buttons()”. The parameters under this widget are the same as before. But, in addition to this, it has a “command” parameter which will call the “click()” function. It is a UDF that consists of the block of code which will add the actual functionalities of the calculator. With that, we will set the positions for the buttons. To get the buttons systematically , according to the size of the window, we will use a condition. The condition says that if the column exceeds 7 then the row must get changed to place another button. That’s how we will be able to see all the buttons on the window.

The last thing is to add the functionalities, we will make a UDF named “click()”. Under this, with the help of an “if-else” ladder, we will check for the buttons that get pressed. First, we will get the information stored in the variable about the type of button pressed. To handle any of the syntax errors while calculating we will run a try and except block.

The first button stated “C” which is for clearing the last digit. To get this task done, we will first delete the last entered value by slicing. The next step is common to all operations, for displaying the result, we first have to delete the whole thing and then insert that particular result and this will be possible by “.delete()” & “.insert()”. The result will get stored in the variable.
Next button “CE”, to clear everything. It is being done by “.delete(0,” end”)”. The parameters passed state that the particular must get deleted from starting to end
The “square root” functionality is being added by using a function from the math module i.e. “.sqrt()”. The values passed under this function as parameters are under the “eval()” function which will allow the evaluation of arbitrary Python expressions from a string-based or compiled-code-based input.
Same as for all the other buttons such as, we will use the functions from the 
# math module.
pi: math.pi

sinh: math.sinh()

cosh: math.cosh()

tanh: math.tanh()

cosθ: math.cos()

sinθ: math.sin()

tanθ: math.tan()

ln: math.log2()

deg: math.degrees()

rad: math.radians()

e: math.e

log10: math.log10()

x!: math.factorial()
