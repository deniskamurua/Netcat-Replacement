# Netcat-Replacement
A python netcat like listener Usage:

python netcat.py --help
usage: netcat.py [-h] [-c] [-e EXECUTE] [-l] [-p PORT] [-t TARGET] [-u UPLOAD]
BHP Net Tool
optional arguments:
-h, --help
show this help message and exit
-c, --command
initialize command shell
-e EXECUTE, --execute EXECUTE
execute specified command
-l, --listen
listen
-p PORT, --port PORT specified port
-t TARGET, --target TARGET
specified IP
-u UPLOAD, --upload UPLOAD
upload file
Example:
netcat.py -t 192.168.1.108 -p 5555 -l -c # command shell
netcat.py -t 192.168.1.108 -p 5555 -l -u=mytest.txt # upload to file
netcat.py -t 192.168.1.108 -p 5555 -l -e="cat /etc/passwd" # execute command
echo 'ABCDEFGHI' | ./netcat.py -t 192.168.1.108 -p 135
# echo local text to server port 135
netcat.py -t 192.168.1.108 -p 5555 # connect to server
