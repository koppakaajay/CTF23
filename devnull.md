# Challenge Description
Given a webpage that shows 500 Internal Server Error. We have to retrieve the error file.
# Approach
The page tells us that the files will be taken from /home/app/uploads.
Using certain commands we can coerce the website into revealing data or running scripts.

Changing the url to `check?file=../../../home/app/app.js` we are taken to a html page with js code.

Inspecting the code we see that it reads a file "/var/log/apache2/error.log"

Changing the url to `check?file=../../../var/log/apache2/error.log` we can access the error log and get the flag.
# Flag Found
flag{wnOzw8egpk8+ieYl+Xytqw==}
