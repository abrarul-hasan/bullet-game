# bullet-game

import pygame

screen_size = [360, 600]
screen = pygame.display.set_mode(screen_size)
background = pygame.image.load('background.png')
planet = pygame.image.load('p_one.png')

spaceship = pygame.image.load('spaceship.png')
bullet = pygame.image.load('bullet.png')

keep_alive = True
while keep_alive:
    pygame.event.get()
    keys = pygame.key.get_pressed()
    if keys[pygame.K_SPACE] == True:
        print('Space key pressed')


    screen.blit(background, [0, 0])


    screen.blit(planet, [140, 50])
    screen.blit(bullet, [180, 500])
    screen.blit(spaceship, [160, 500])
    pygame.display.update()
