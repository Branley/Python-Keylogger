<h1>Python Keylogger Program</h1>

<h2>Description</h2>
In this program, I learned to code a Keylogger in Python. The program records keystrokes on a computer and does so by capturing keys pressed on the keyboard. The data is logged and can be used for monitoring purposes. In the wrong hands, hackers can use this program to acquire 
personal information such as passwords and credit card information.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Python Language</b>

<h2>Environments Used </h2>

- <b>Visual Studio Code</b> 

<h2>Lab walk-through:</h2>

<p align="center">
Step 1: <br/>
Pi inputs a library and includes a keyboard module to capture key events from the user.
To use this library, you could type "py -m pip install pynput" inside the terminal of vs code. 
<img src="https://i.imgur.com/3CGT8Hk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Step 2:  <br/>
This defines the main method that launches when the program fires. For example, if the main method is ready to launch, what do we want it to do?
to do? 
<br/>
<img src="https://i.imgur.com/s5riGi3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 3: <br/>
Continuing from step 2, this is what we are going to do. Listener is the object we are creating. With keyboard.listener, we have to pass in parameters inside the parenthesis. What is inside the parenthesis is that the listener is turned on and when a user types 
something on the keyboard, wherever it is directed to, thats where we are going to send the event. "on_press = keyboard" means everytime a key is pressed, pass that information to this keypressed function.
<img src="https://i.imgur.com/z2O5PYB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 4: <br/>
We added 2 new lines to use our object. "Listener.start()" starts the listener for the keyboard method to start capturing the key events. "input()" tells python the we are ready to start asking for strings down in the terminal.
<img src="https://i.imgur.com/6ZALjXV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 5: <br/>
Here is where we define our function. The parameter "key" is given by default so it does not need to be specified. "print(str(key))" makes sure the key is converted to a string so that it can be printed to the terminal.
<img src="https://i.imgur.com/AJ9INqo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 6: <br/>
Now we have to write these key events to a text file. "with open" is a method to open, create, and edit files. Inside the parenthesis is where we named the file "keyfile.txt". The 'a' that follows in the line appends or add to the file's existing content. "as logKey"
serves as a reference for later. </br>
<img src="https://i.imgur.com/iLZtbjN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 7: <br/>
In the try area, we are converting this key to a character to put into our file. The reason why this is in a try and expect block is becauase "char = key.char" does not always work and sometimes comes out with errors. To go around that, "print("error getting char)"
is the expection and we just printed it to ourselves.
<img src="https://i.imgur.com/SnAjJBn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 8: </br>
Hit run and start typing. You will see that the program is capturing the keystrokes of your keyboard. 
</p>

