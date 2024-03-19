# Jinelle Flores Etienne
# Ingeniería en Tecnologías Computacionales
# Tampico, Tamaulipas
## - Equipo - 
# **Semana Tec**

# Nueva branch

Emojis
💟♥️💻

# 2. Tipos de letra
**Bold**
*Italic*
> Block

> Hola
> Adios

# 3. Lista enumerada
1. Uno
2. Dos
3. Tres

# 4. Lista con viñetas
- Uno
- Dos
- Tres

# 5. Código
```python
from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```

# 6. Regla
---

# 7. Link
[Free Games](https://grantjenks.com/docs/freegames/)

[Markdown](https://grantjenks.com/docs/freegames/](https://www.markdownguide.org/cheat-sheet/)https://www.markdownguide.org/cheat-sheet/)

# 8. Imágenes
##Tampico
![Tampico](https://github.com/Jinellie/RepoSemanaTec/assets/89491839/524a383c-cb5d-4ea7-9598-85dbb7db6ad9)

# 9. Tabla

| Columna1 | Columna 2 |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

# 10. Lista de equipo
- [x] Jinelle Flores Etienne
- [x] Melissa Salazar
- [x] Roberta González
