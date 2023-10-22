# Install Pygame
The easist way to install pygame is by using a Python package manager such as pip or Anaconda. Using pip we have
```Shell
pip install pygame
```
## Basics
### Initialization
We initialize a new instance via
```Python
import pygame

pygame.init()
```
### Set caption of the game
We set the caption as follows
```Python
import pygame

pygame.init()
canvas = pygame.display.set_caption("Name of the Game")
```
### Create canvas
```Python
WIDTH = 800
HEIGHT = 500
# Set size of canvas
canvas = pygame.display.set_mode((WIDTH, HEIGHT))
# Fill canvas
background_color = (255, 255, 255)
canvas.fill(background_color)
```
### Game loop
The basic loop for the game is given by
```Python
running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False
    pygame.display.update()
```
We may also exit the game via the following statements
```Python
while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            quit()
    pygame.display.update()
```
### Pygame time
```Python
# Creating a clock in pygame
clock = pygame.time.Clock()
# Adding time to the clock, e.g. 60fps
clock.tick(60)
```

### Pygame color
We can define different colors in pygame as follows
```Python
color_black = pygame.Color(0, 0, 0)
color_red = pygame.Color(255, 0, 0)
```

### Images in pygame
We can load and display images via
```Python
game_image = pygame.image.load("path_to_image")
```

## Event handling
We check for keyboard events within the game event loop as follows
```Python
while True:
    for event in pygame.event.get():
        if event.type == pygame.KEYDOWN:
            if event.key == pygame.K_UP:
                change_to = 'UP'
            if event.key == pygame.K_DOWN:
                change_to = 'DOWN'
            if event.key == pygame.K_LEFT:
                change_to = 'LEFT'
            if event.key == pygame.K_RIGHT:
                change_to = 'RIGHT'
```

```Python
```

```Python
```
