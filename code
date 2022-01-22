import pygame
import random
import time
import numpy as np
# lol this is very messy code didnt have enough time to clean it
# importing all libraries
Y2 = 600
X2 = 400
X3 = 400
Y3 = 600
X4 = 140
Y4 = 50
#setting X and Y for caption on screen
score_color = (255, 165, 0)
X = 140
sqa = 0
Green = (0, 255, 0)
Red = (255, 0, 0)
Y = 50
size = 3
level = 1
BLACK = pygame.Color(0, 0, 0)
WHITE = pygame.Color(255, 255, 255)
SPcolor = tuple(np.random.randint(0, 255, size))
pygame.init()
width = 400
height = 400
screen = pygame.display.set_mode((width, height))
#setting the screen height and width
pygame.display.set_caption('Collision')
playerspeed = -0.1
playerspeedb = 0.1
BGC = (0, 0, 0)
score_font = pygame.font.SysFont("Times New Roman", 20)
score_font2 = pygame.font.SysFont("Verdana", 20)



# create the pads Rect
playerposX = 0
playerposY = random.randint(0,400)
right_pad = pygame.Rect(10, 10, 0, 0)
playerX = 300
player2X = 400
player3X = 490
player4X = 560
player5X = 660
player6X = 500
player7X = 300
player8X = 400
player9X = 490
player10X = 500
player11X = 510
player12X = 560
player13X = 520
player14X = 400
player15X = 600
player16X = 560
player17X = 640
player18X = 610
#setting the player X POS
  # create the square Rect
playerY = random.randint(0,370)
playerY2 = random.randint(0,370)
playerY3 = random.randint(0,370)
playerY4 = random.randint(0,370)
playerY5 = random.randint(0,370)
playerY6 = random.randint(0,370)
playerY7 = random.randint(0,370)
playerY8 = random.randint(0,370)
playerY9 = random.randint(0,370)
playerY10 = random.randint(0,370)
playerY11 = random.randint(0,370)
playerY12 = random.randint(0,370)
playerY13 = random.randint(0,370)
playerY14 = random.randint(0,370)
playerY15 = random.randint(0,370)
playerY16 = random.randint(0,370)
playerY17 = random.randint(0,370)
playerY18 = random.randint(0,370)
#setting player Y
bulletX = 100

square = pygame.Rect(playerX, playerY, 20, 20)
right_bound = pygame.Rect(-100, 0, 100, 500)
left_bound = pygame.Rect(790, 0, 100, 500)
square2 = pygame.Rect(player2X, playerY2, 40, 40)
square3 = pygame.Rect(player3X, playerY3, 20, 50)
square4 = pygame.Rect(player4X, playerY4, 60, 30)
square5 = pygame.Rect(player5X, playerY5, 20, 20)
square6 = pygame.Rect(player6X, playerY6, 20, 30)
square7 = pygame.Rect(player7X, playerY7, 40, 40)
square8 = pygame.Rect(player8X, playerY8, 20, 50)
square9 = pygame.Rect(player9X, playerY9, 60, 30)
square10 = pygame.Rect(player10X, playerY10, 20, 20)
square11 = pygame.Rect(player11X, playerY11, 20, 30)
square12 = pygame.Rect(player12X, playerY12, 40, 40)
square13 = pygame.Rect(player13X, playerY13, 20, 50)
square14 = pygame.Rect(player14X, playerY14, 60, 30)
square15 = pygame.Rect(player15X, playerY15, 20, 20)
square16 = pygame.Rect(player16X, playerY16, 20, 30)
square17 = pygame.Rect(player17X, playerY17, 40, 40)
square18 = pygame.Rect(player18X, playerY18, 20, 50)
# drawing and initializing the objects 

playerX_change = 0

velocity_x = -0.15
velocity_2x = -0.15
velocity_3x = -0.15
velocity_4x = -0.15
velocity_5x = -0.15
velocity_6x = -0.15
velocity_7x = -0.15
velocity_8x = -0.15
velocity_9x = -0.15
velocity_10x = -0.15
velocity_11x = -0.15
velocity_12x = -0.15
velocity_13x = -0.15
velocity_14x = -0.15
velocity_15x = -0.15
velocity_16x = -0.15
velocity_17x = -0.15
velocity_18x = -0.15
# vel of squares and etc
clock = pygame.time.Clock()
bullet = pygame.Rect(bulletX, playerposY + 10, 10, 10)
x1_move = 0
y1_move = 0
# USing Delta time as a frame rate
while True:

    screen.fill(BLACK) 
    
    bullet = pygame.Rect(bulletX, playerposY +10, 40, 10)
    pygame.draw.rect(screen, SPcolor, bullet)
    x1 = width / 2
    y1 = height / 2
    left_pad = pygame.Rect(110, playerposY, 50, 50)
    # setting screen as black and laying out the left_pad basics

    pygame.draw.rect(screen, SPcolor, square)
    pygame.draw.rect(screen, SPcolor, square2) 
    pygame.draw.rect(screen, SPcolor, square3) 
    pygame.draw.rect(screen, SPcolor, square4) 
    pygame.draw.rect(screen, SPcolor, square5) 
    pygame.draw.rect(screen, SPcolor, square6)
    pygame.draw.rect(screen, SPcolor, square7)
    pygame.draw.rect(screen, SPcolor, square8) 
    pygame.draw.rect(screen, SPcolor, square9) 
    pygame.draw.rect(screen, SPcolor, square10) 
    pygame.draw.rect(screen, SPcolor, square11) 
    pygame.draw.rect(screen, SPcolor, square12)
    pygame.draw.rect(screen, SPcolor, square13)
    pygame.draw.rect(screen, SPcolor, square14) 
    pygame.draw.rect(screen, SPcolor, square15) 
    pygame.draw.rect(screen, SPcolor, square16) 
    pygame.draw.rect(screen, SPcolor, square17) 
    pygame.draw.rect(screen, SPcolor, square18)
    # drawing all the squares on the screen
    dt = clock.tick(100)
    
    time1 = 0
    value = score_font.render("LEVEL: " + str(level), True, score_color)
    value2 = score_font.render("# of squares: " + str(sqa), True, score_color)
    value3 = score_font2.render("You WIN", True,   score_color)
    value4 = score_font2.render("You Lost", True, score_color)
    # diff captions

    textRect = value.get_rect()
    textRect.center = (X // 2, Y // 2) 
    textRect2 = value2.get_rect()
    textRect2.center = (X2 // 2, Y2 // 2) 
    textRect3 = value3.get_rect()
    textRect3.center = (X3 // 2, Y3 // 2) 
    textRect4 = value4.get_rect()
    textRect4.center = (X4 // 2, Y4 // 2) 



    
    event = pygame.event.poll()

    if event.type == pygame.KEYDOWN:

      if event.key == pygame.K_w:
        playerposY -= 30


      if event.key == pygame.K_s:
        playerposY += 30
      
      if event.key == pygame.K_SPACE:
        playerX_change = -5
    if event.type == pygame.KEYUP:
      if event.key == pygame.K_SPACE:
        bulletX = 110
        playerX_change = 0

      if playerposY >= 369:
        playerposY = 369
      if playerposY <= 0: 
        playerposY = 0
      if event.type == pygame.QUIT:
        break
    bulletX -= playerX_change
    # use the move function inplace
    square.move_ip(velocity_x * dt, 0)
    square2.move_ip(velocity_2x * dt, 0)
    square3.move_ip(velocity_3x * dt, 0)
    square4.move_ip(velocity_4x * dt, 0)
    square5.move_ip(velocity_5x * dt, 0)
    square6.move_ip(velocity_6x * dt, 0)
    square7.move_ip(velocity_7x * dt, 0)
    square8.move_ip(velocity_8x * dt, 0)
    square9.move_ip(velocity_9x * dt, 0)
    square10.move_ip(velocity_10x * dt, 0)
    square11.move_ip(velocity_11x * dt, 0)
    square12.move_ip(velocity_12x * dt, 0)
    square13.move_ip(velocity_13x * dt, 0)
    square14.move_ip(velocity_14x * dt, 0)
    square15.move_ip(velocity_15x * dt, 0)
    square16.move_ip(velocity_16x * dt, 0)
    square17.move_ip(velocity_17x * dt, 0)
    square18.move_ip(velocity_18x * dt, 0)
   # moving squares with function in pygame


    
    # draw using the rect



   
    # draw the pads

    pygame.draw.rect(screen, WHITE, left_pad)
    pygame.draw.rect(screen, WHITE, right_pad)

    pygame.draw.rect(screen, WHITE, left_bound)
    pygame.draw.rect(screen, WHITE, right_bound)
    if square.colliderect(left_bound):
      level += 1
      playerspeed -= 0.002
      velocity_x = playerspeed
    if square2.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_2x = playerspeed
    if square3.colliderect(left_bound):
      playerspeed -= 0.002      
      velocity_3x = playerspeed
    if square4.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_4x = playerspeed
    if square5.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_5x = playerspeed
    if square6.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_6x = playerspeed
    if square7.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_7x = playerspeed
    if square8.colliderect(left_bound):
      playerspeed -= 0.002      
      velocity_8x = playerspeed
    if square9.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_9x = playerspeed
    if square10.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_10x = playerspeed
    if square11.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_11x = playerspeed
    if square12.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_12x = playerspeed
    if square13.colliderect(left_bound):
      playerspeed -= 0.002      
      velocity_13x = playerspeed
    if square14.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_14x = playerspeed
    if square15.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_15x = playerspeed
    if square16.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_16x = playerspeed
      level += 1 
    if square17.colliderect(left_bound):
      playerspeed -= 0.002
      velocity_17x = playerspeed
    if square18.colliderect(left_bound):
      playerspeed -= 0.002 
      level += 1     
      velocity_18x = playerspeed
      # if hits side then speeds up and increases level
    # lol this is such messy code
    
    if square.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_x = playerspeedb
    if square2.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_2x = playerspeedb
    if square3.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_3x = playerspeedb
    if square4.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_4x = playerspeedb
    if square5.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_5x = playerspeedb
    if square6.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_6x = playerspeedb
    if square7.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_7x = playerspeedb
    if square8.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_8x = playerspeedb
    if square9.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_9x = playerspeedb
    if square10.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_10x = playerspeedb
    if square11.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_11x = playerspeedb
    if square12.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_12x = playerspeedb
    if square13.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_13x = playerspeedb
    if square14.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_14x = playerspeedb
    if square15.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_15x = playerspeedb
    if square16.colliderect(right_bound):

      playerspeedb += 0.002
      velocity_16x = playerspeedb
    if square17.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_17x = playerspeedb
    if square18.colliderect(right_bound):
      playerspeedb += 0.002
      velocity_18x = playerspeedb
   

    if left_pad.colliderect(square):
      velocity_x = 0.1

    if left_pad.colliderect(square2):
      velocity_2x = 0.1 

 
    if left_pad.colliderect(square3):
      velocity_3x = 0.1   

    if left_pad.colliderect(square4):
      velocity_4x = 0.1    

    if left_pad.colliderect(square5):
      velocity_5x = 0.1  

    if left_pad.colliderect(square6):
      velocity_6x = 0.1

      # if the squares collide with bullet then they dissapear
    if bullet.colliderect(square):
      sqa += 1
      velocity_x = 0.1
      square = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square2):
      sqa += 1
      velocity_2x = 0.1 
      square2 = pygame.Rect(0, 0, 0, 0)
 
    if bullet.colliderect(square3):
      sqa += 1
      velocity_3x = 0.1   
      square3 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square4):
      sqa += 1
      velocity_4x = 0.1    
      square4 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square5):
      sqa += 1
      velocity_5x = 0.1  
      square5 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square6):
      sqa += 1
      velocity_6x = 0.1
      square6 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square7):
      sqa += 1
      square7 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square8):
      sqa += 1
      square8 = pygame.Rect(0, 0, 0, 0)
 
    if bullet.colliderect(square9):
      sqa += 1
      square9 = pygame.Rect(0, 0, 0, 0)
 
    if bullet.colliderect(square10):
      sqa += 1
      square10 = pygame.Rect(0, 0, 0, 0)
 
    if bullet.colliderect(square11):
      sqa += 1
      square11 = pygame.Rect(0, 0, 0, 0)
 
    if bullet.colliderect(square12):
      sqa += 1
      square12 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square13):
      sqa += 1
      square13 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square14):
      sqa += 1
      square14 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square15):
      sqa += 1
      square15 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square16):
      sqa += 1
      square16 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square17):
      sqa += 1
      square17 = pygame.Rect(0, 0, 0, 0)
    if bullet.colliderect(square18):
      sqa += 1
      square18 = pygame.Rect(0, 0, 0, 0)
    if sqa > 17:
      screen.fill(Green)
      score_font = pygame.font.SysFont("Times New Roman", 0)
      screen.blit(value3, textRect3)

    # explanitory
    if level > 80:
      screen.fill(Red)
      score_font = pygame.font.SysFont("Times New Roman", 0)
      screen.blit(value4, textRect4)
  
    if bulletX > 350:
      bulletX = 100
    screen.blit(value, textRect)
    screen.blit(value2, textRect2)
   

    pygame.display.flip()
  
