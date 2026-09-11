# Manual Práctico del Editor VI

![vi](https://img.shields.io/badge/editor-vi-brightgreen)
![Linux](https://img.shields.io/badge/OS-Linux-blue)
![Estado](https://img.shields.io/badge/estado-completado-green)

Manual interactivo sobre el uso del editor `vi` desarrollado para la asignatura Seminario Linux.

## Tabla de Contenido
1. [Modos de trabajo y creación](docs/01-modos-y-creacion.md)
2. [Navegación básica](docs/02-navegacion.md)
3. [Edición y deshacer](docs/03-edicion-y-deshacer.md)
4. [Copiar y pegar](docs/04-copiar-y-pegar.md)
5. [Buscar y reemplazar](docs/05-buscar-y-reemplazar.md)
6. [Insertar texto](docs/06-insertar-texto.md)
7. [Guardar y salir](docs/07-guardar-y-salir.md)

## ¿Qué es vi?
`vi` es uno de los editores de texto en terminal más populares y fundamentales del mundo Unix/Linux. A diferencia de un editor gráfico tradicional, su funcionamiento se basa en modalidades que permiten navegar, editar y manipular texto de manera muy rápida sin tocar el ratón.

Aprender `vi` es esencial para cualquier desarrollador o administrador de sistemas, ya que está presente por defecto en prácticamente cualquier servidor Linux.

## Tabla Resumen (Cheat Sheet)

| Categoría | Comando | Qué hace | Ejemplo propio |
| :--- | :--- | :--- | :--- |
| **Modos** | `i` | Entra al modo inserción antes del cursor | `i` para empezar a escribir texto normal |
| **Modos** | `Esc` | Vuelve al Modo Normal | `Esc` para salir del modo inserción y dar órdenes |
| **Navegación** | `h`, `j`, `k`, `l` | Mueve el cursor (izq, abajo, arriba, der) | Usar `j` para bajar de línea en el archivo |
| **Navegación** | `w` / `b` | Avanza / retrocede una palabra | `w` para saltar rápido a la siguiente palabra |
| **Navegación** | `0` / `$` | Va al inicio / final de la línea | `$` para saltar directo al final de la frase |
| **Navegación** | `gg` / `G` | Va a la primera / última línea del archivo | `G` para ir rápido al final del documento |
| **Edición** | `x` | Borra el carácter bajo el cursor | `x` sobre una letra equivocada para eliminarla |
| **Edición** | `dw` | Borra la palabra completa | `dw` sobre la palabra 'error' para borrarla |
| **Edición** | `dd` | Borra o corta la línea entera | `dd` sobre una línea que quiero eliminar |
| **Edición** | `u` | Deshace el último cambio | Presiono `u` si borré una línea sin querer |
| **Copiar/Pegar**| `yy` | Copia la línea actual | `yy` para guardar la línea en el portapapeles |
| **Copiar/Pegar**| `yw` | Copia la palabra actual | `yw` para duplicar solo una palabra |
| **Copiar/Pegar**| `p` / `P` | Pega el texto abajo / arriba del cursor | `p` para pegar una línea copiada abajo |
| **Búsqueda** | `/texto` | Busca una palabra hacia adelante | `/Linux` para encontrar esa palabra |
| **Búsqueda** | `:%s/a/b/g` | Reemplaza 'a' por 'b' en todo el archivo | `:%s/error/fix/g` corrige todas las coincidencias |
| **Inserción** | `a` / `A` | Inserta después del cursor / al final de línea | `A` para agregar texto al final sin moverme |
| **Inserción** | `o` / `O` | Abre nueva línea abajo / arriba para escribir | `o` para empezar a redactar un párrafo nuevo abajo |
| **Guardado** | `:w` | Guarda los cambios sin salir | `:w` para salvar mi avance mientras trabajo |
| **Guardado** | `:wq` | Guarda los cambios y sale del editor | Usado al terminar de redactar cada nota |
| **Guardado** | `:q!` | Sale forzadamente sin guardar | `:q!` si cometí errores y quiero descartarlos |

## Créditos
* **Asignatura:** Seminario Linux 
* **Docente:** Bayron Jesit Ospina Cifuentes
* **Estudiante:** David Gomez Jimenez
