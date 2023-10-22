# Install Pygame
The easist way to install pygame is by using a Python package manager such as pip or Anaconda. Using pip we have
```Shell
pip install pygame
```
## Basics
### Initialization
We can initialize the game as follows
```Python
import pygame

pygame.init()
canvas = pygame.display.set_mode((500, 500))
pygame.display.set_caption("My Board")

exit = False

while not exit:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            exit = True
    pygame.display.update()
```
### Create canvas
```Python
WIDTH = 800
HEIGHT = 500
canvas = pygame.display.set_mode((WIDTH, HEIGHT))
```

### Pygame time
```Python
# Creating a clock in pygame
clock = pygame.time.Clock()
# Adding time to the clock, e.g. 60fps
clock.tick(60)
```

```Python
```

```Python
```

```Python
```

```Python
```
