  Let's play around with CyberChef a little bit. At first glance, we see the data is displayed in 16 characters, AKA hex. Let's decode that.
  
  <img src="https://user-images.githubusercontent.com/9062530/209875387-9102ccbd-2adf-4972-bfec-836ad20d326b.png">

  Next, we see that some characters are grouped as if they are already in the form of words. This is likely a weak caesar or rotating cipher. After playing around for a while, we see that using rotating the alphabet 13, then 47, then 13 times again gives us a message and a flag! (ROT13, ROT47, ROT13)

  The message we recieved from the last flag was weird. It mentioned a padlock and we know this is a steg room, so let's download the room icon and extract exif data from it.
  
  <img src="https://user-images.githubusercontent.com/9062530/209875037-26cc3144-ece6-4c2b-ba02-d71981831276.png">

  That is weird. It says there is a trailer on the data. Let's open it with a hex editor and check it out.
  
  <img src="https://user-images.githubusercontent.com/9062530/209876006-c8c01936-6b9a-4a40-bb4a-daedb2bb0345.PNG">

  There, we have the last flag!
