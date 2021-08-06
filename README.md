# BHP2-Code

Basically I will be adding my compiled "netcat.py" from the Black Hat Python 2nd Edition book. Will also continue updating it to my comfort. If you can help in writing better code, you're more than welcome to do so. I want to improve my coding habits.

# Usage
Usage: linux_nc [-h] [-c] [-e EXECUTE] [-l] [-p PORT] [-t TARGET] [-u UPLOAD]

BHP Net Tool

optional arguments:

  -h, --help            show this help message and exit
  
  -c, --command         command shell
  
  -e EXECUTE, --execute EXECUTE execute specified command
  
  -l, --listen          listen
  
  -p PORT, --port PORT  specified port
  
  -t TARGET, --target TARGET     specified IP
  
  -u UPLOAD, --upload UPLOAD upload file
  

Example: 2 

            ./linux_nc -t 192.168.1.108 -p 5555 -l -c #command shell 
            
            ./linux_nc -t 192.168.1.108 -p 5555 -l -u=mytest.txt # upload to file 
            
            ./linux_nc -t 192.168.1.108 -p 5555 -l -e="cat /etc/passwd" # execute command 
            
            echo 'ABC' | ./linux_nc -t 192.168.1.108 -p 135 # echo text to server port 135 
            
            ./linux_nc -t 192.168.1.108 -p 5555 # connect to server 
            

# Disclaimer
THIS IS FROM THE BLACK HAT PYTHON 3 BOOK.
