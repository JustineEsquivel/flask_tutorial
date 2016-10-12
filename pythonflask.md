#How to set up set-up a flask website

###This tutorial will cover how to to set-up your very own website using your terminal, a text editor, Raspberry Pi and Flask. It may seem daunting, but trust us, the outcome is worth it! 

##Install Flask

1. Open your terminal
2. Install Flask by typing sudo apt-get install python3-flask
3. Open Ipython3 in the terminal by directly typing 'ipython3'


##When Flask is installed

1. Open a new project in a text editor and paste in: 

from flask inport Flask

app = Flask(_name_)

@app.route('/')
def index():
    return 'Hello world'
    
if_name_ == '_main_':
    app.run(debug=True, host='0.0.0.0')
    
2. Save this file as app.py
3. Open a new tab in the terminal (bash)
4. Type 'run app.py'
5. To copy Flask onto your Raspberry pi type 'scp app.py + your ssh IP address + computer’s username 

If you did this right the following should appear: 

* Running on http://0.0.0.0:5000/
* Restarting with reloader

##Now it's pointing to the Raspberry Pi. How do you point it somewhere else, like your own computer? Great question! 

### Open up a new bash tab
in bash write
 ``` ifconfig <b>tag</b> ```
 copy and paste the __computer IP address and username__ in a text file somwhere
 _usersname will end in $_
 
 Back in the Rasberry Pi tab write
  ``` scp index.html ‘COMPUTER NAME’@’COMPUTER IP ADDRESS’:‘PATH TO FILE
 <b>tag</b> ```
 
 ## Get file back to Rasberry Pi
 ###   ``` Scp index.html ‘computer name’@’raspberrypi IP adress’:/Users/name/file location…. (wherever you saved index.html)/new name for your file
 <b>tag</b> ```
 
If you did this right you will be prompted for your computer password 
LS to show that index has now been placed onto your raspi

##To rename and/or move new index.html

### Delete existing index.html
``` Sudo nano rm -v index.html <b>tag</b> ```

Move new index.html into home directory
``` cd <b>tag</b> ``` into new directory where new index.html is
``` mv file index.html ~ <b>tag</b> ``` to put new index.html onto home directory to become new index.html file
To double check preview index.html in text editor

##### YOU MADE IT BITCH

