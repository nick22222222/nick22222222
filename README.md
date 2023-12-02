- 👋 Hi, I’m @nick22222222
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
nick22222222/nick22222222 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

import pygame


pygame.init()

screen_width = 800
screen_height = 800

screen = pygame.display.set_mode((screen_width, screen_height))

font =pygame.font.SysFont("Intro", 40)
img = pygame.image.load("1.JPG")

img = pygame.transform.scale(img, (134, 120))

while True:
    for event in pygame.event.get():
          if event.type == pygame.QUIT:
              pygame.quit()
              quit()
    text = font.render("START", True, (32, 233, 32))
    screen.blit(text, (50, 70))
