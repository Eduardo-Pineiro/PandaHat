You download an image that seems very very corrupted. I tried exif data, and outguess and stegseek but found nothing. I then checked the strings and found a very funky line, 

![1](./Images/UnFormat_1.png)

The file contained plain text that read corrupted. I took a gamble and used nano to remove these lines and while the file is still corrupt, i saw an image in the small icon. If you zoom in you see the flag

![2](./Images/UnFormat_2.png)
