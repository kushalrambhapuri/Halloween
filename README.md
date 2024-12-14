# Halloween Prank
Looking to give your friends a good scare this Halloween? With just 15 lines of Python, you can create a chilling prank featuring a jump scare image and creepy sounds!

Requirements
Python Installed on your computer
Pygame Library (Install it using pip install pygame)
A scary image file (scr.jpg) and two sound files (ratsasan.mp3 and scary.mp3)
Step-by-Step Guide
Step 1: Install Pygame
Open your terminal or command prompt and run:

pip install pygame  
Step 2: Write the Code
Here’s the Python script for the prank:

import pygame  
from time import sleep  

pygame.init()  

Set up a fullscreen window  
window = pygame.display.set_mode((0, 0), pygame.FULLSCREEN)  

Initialize the mixer for sounds  
pygame.mixer.init()  

Play the first sound  
pygame.mixer.music.load('ratsasan.mp3')  
pygame.mixer.music.play()  
sleep(5)  # Let the first sound play for 5 seconds  

Play the scary sound and display the jump scare image  
pygame.mixer.music.load('scary.mp3')  
pygame.mixer.music.play()  
sleep(1)  
image = pygame.image.load('scr.jpg')  
window.blit(image, (0, 0))  
pygame.display.update()  
sleep(3)  # Keep the image on screen for 3 seconds  
Step 3: Prepare the Files
Place the ratsasan.mp3 (creepy background sound), scary.mp3 (jump scare sound), and scr.jpg (scary image) in the same directory as your script.
Ensure the files are correctly named and compatible.
How It Works
The program starts by playing an eerie sound (ratsasan.mp3) for 5 seconds.
After that, a jump scare sound (scary.mp3) plays, and the screen displays a fullscreen scary image (scr.jpg).
The jump scare lasts for 3 seconds before the program ends.
Run the Prank
Save the script in a file named halloween_prank.py.
Run it using your Python editor or terminal.
Watch your friends jump out of their seats when the prank kicks in!
Important Notes
Prank Responsibly: Use this prank only on friends who can handle it.
Close the Program: Press Ctrl+Alt+Del (Windows) or Command+Option+Esc (Mac) to close the program if needed.
Have fun scaring your friends this Halloween! 👻🎃
