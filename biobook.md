BioBook
Challenge Description
Given a website which contains biographies of celebrities from which we need to find the flag.

Approach:
Initial Analysis:
Opening the challenge instance takes us to a site containing the biography of Robert Downey Jr.

Clicking on 'Read More' takes us to a more detailed Biography of RDJ.

Changing Object Reference:
After Inspecting the url I noticed the object reference parameter Bio?id=1
Changing the id to 0 we get a page with information regarding IDOR.
We can change the id values from 1-6 to read other biographies.

The flag is at the end of the page.
# Flag Found
Flag: flag{1ysHPBbW/UluTliEloYl8w==}
