# Challenge Description
The challenge is to unravel the hidden information within the image
# Approach
Read the resources given for this challenge. Found a chall.png file in the attachments folder. at first i used all the image stegonography tools like png check, tweak png,stegsolve, stegnographer, etc but none of them worked. 

So I tried using screening tools and found two intresting tools. One of them is Ghex. So i used ghex to get the hex data of the image and I realised its harder to understand search dor something in it. So i used an online hexeditor called hexed.it. There I noticed there are two IEND chunks. Upon further investigation I found that there was some wave format file inscribed into that image

So I used the other tool called binwalk using the command `binwalk -e chall.png` to extract the contents, but I got some error as I was running it in root terminal, so I found that we need use the command `binwalk -e chall.png --run-as=root`. And found the secret.wav file, which was an audio file. I listened to the audio and I found nothing I tried a lot of ways thinking if it was some code but none of them worked.

So I read about the audio forensice from wiki.bi0s.in and learned about sonic-visualiser. Hence I installed it and ran it using the command `sonic-visualiser chall.png` and found this challenge was similar to what it is mentioned in the website. So I navigated to layers tab and clicked on add spectogram layer and found the flag after zomming it in and out.
# Flag found
`bi0s{th4t_w4s_4_l0t_0f_w4v3s_62859}`
