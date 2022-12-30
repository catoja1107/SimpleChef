  All we are given at the start of this room is this data in Task 1:
  
<img height="50%" width="50%" src="https://user-images.githubusercontent.com/9062530/210106405-33c30d6b-9f09-47a7-b763-21acc5df3fa0.png">

  Let's play around with CyberChef a little bit. At first glance, we see the data range is from 1-f. It is base 16, AKA hexadecimal. Let's decode that.
  
  <img src="https://user-images.githubusercontent.com/9062530/209875387-9102ccbd-2adf-4972-bfec-836ad20d326b.png">

  Next, we see that some characters are grouped as if they are already in the form of words. This is likely a weak caesar or rotating cipher. After playing around for a while, we see that using rotating the alphabet 13, then 47, then 13 times again gives us a message and a flag! (ROT13, ROT47, ROT13)

  The message we recieved from the last flag was weird. It mentioned a padlock and we know this is a steg room, so let's download the room icon and extract exif data from it.
  
  <img alt="SimpleChef room icon" src="https://user-images.githubusercontent.com/9062530/210106691-1ee7ca6c-2c88-475e-824e-aa3a0c506d17.png">

  
  <img src="https://user-images.githubusercontent.com/9062530/209875037-26cc3144-ece6-4c2b-ba02-d71981831276.png">

  That is weird. It says there is a trailer on the data. Let's open it with a hex editor and check it out.
  
  <img src="https://user-images.githubusercontent.com/9062530/209876006-c8c01936-6b9a-4a40-bb4a-daedb2bb0345.PNG">

  There, we have the last flag!

<!-- Hello, traveler. Please ignore this HTML/Markdown monstrocity.

    ,                      _,-
   (\                  _,-','
    \\              ,-"  ,'
     \\           ,'   ,'
      \\        _:.----__.-."-._,-._
       \\    .-".:--`:::::.:.:'  )  `-.
        \\   `. ::L .::::::'`-._  (  ) :
         \\    ":::::::'  `-.   `-_ ) ,'
          \\.._/_`:::,' `.     .  `-:
          :" _   "\"" `-_    .    `  `.
           "\\"":--\     `-.__ ` .     `.
             \\'::  \    _-"__`--.__ `  . `.     _,--..-
              \\ ::  \_-":)(        ""-._ ` `.-''
               \\`:`-":::/ \\ .   .      `-.  :
               :\\:::::::'  \\     `    .   `. :
                :\\:':':'  . \\           `,  : :
                : \\     .    \\      .       `. :       ,-
               __`:\\      .   \\ .   `  ,'    ,: :   ,-'
        _,---""  :  \\ '        \\  .          :-"  ,'
    ,-""        :    \\:  .  :   \\  `  '     ,'   /
   '            :  :  \       .   \\   .   _,'  ,-'
               :  .   '       :   :`   `,-' ,--'
                :     :   :      ,'-._,' ,-'
                _:     :        :8:  ,--'
               :dd`-._,'-._.__-""' ,'
                             ,----'
                      _.----'
              __..--""
            ""

-->
