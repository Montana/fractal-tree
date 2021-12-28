# Fractal tree using pygame, math libraries

Run: 

```bash
python tree.py
```
The output should be this: 

<img width="572" alt="Screen Shot 2021-12-28 at 3 15 22 PM" src="https://user-images.githubusercontent.com/20936398/147614072-60fc1a35-2695-44f9-bcc8-666a0798e516.png">

You can achieve different results via editing this portion of Python:

```python
if depth:
  x2 = x1 + int(math.cos(math.radians(angle)) * depth * 10.0)
  y2 = y1 + int(math.sin(math.radians(angle)) * depth * 10.0)
  pygame.draw.line(screen, (255,255,255), (x1, y1), (x2, y2), 2)
  drawTree(x2, y2, angle - 7, depth - 1)
  drawTree(x2, y2, angle + 20, depth - 1)
```

That would print out something like this: 

<img width="587" alt="Screen Shot 2021-12-28 at 3 16 04 PM" src="https://user-images.githubusercontent.com/20936398/147614229-03d8c749-d1fa-485e-a03c-eaa505fb7321.png">

Enjoy.
