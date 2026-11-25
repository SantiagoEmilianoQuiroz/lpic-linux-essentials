# Ejercicios de globbing en Linux

Practica desde esta carpeta. Para comprobar un patrón sin abrir los archivos, puedes ejecutar:

```bash
printf '%s\n' PATRON
```

Reemplaza `PATRON` por el glob que quieras probar. La shell mostrará los nombres que coincidan.

## Ejercicios

1. Muestra todos los archivos con extensión `.txt`.
2. Muestra todos los archivos cuyo nombre empiece por `archivo`.
3. Muestra los archivos `archivo` seguidos de exactamente un carácter y la extensión `.txt`.
4. Muestra `archivo1.txt`, `archivo2.txt` y `archivo3.txt` usando una clase de caracteres.
5. Muestra los archivos `archivo10.txt`, `archivo11.txt` y `archivo12.txt` usando una clase de caracteres.
6. Muestra todos los archivos cuyo nombre empiece por `notas`.
7. Muestra los archivos `notas1.txt` hasta `notas9.txt`, sin incluir `notas10.txt`.
8. Muestra `notas4.txt` hasta `notas8.txt` usando un rango.
9. Muestra todos los logs con extensión `.txt`.
10. Muestra los logs `.txt` cuyo año esté entre 2024 y 2029.
11. Muestra los logs `.txt` de los años 2024, 2025, 2026 y 2027 usando un rango.
12. Muestra los logs `.csv` de los años 2026 a 2029.
13. Muestra los logs `.csv` de los años 2030 a 2035 usando un rango.
14. Muestra los logs `.txt` cuyos nombres tengan exactamente cuatro caracteres en el año.
15. Muestra todos los archivos con extensión `.csv`, incluidos `datos.csv`.
16. Muestra los archivos con extensión `.txt` o `.csv` usando clases de caracteres.
17. Encuentra la imagen `.png` sin escribir su nombre completo.
18. Muestra los archivos `.txt` cuyo nombre contenga el dígito `1`.
19. Muestra el archivo oculto que empieza por `.o`.
20. Muestra todos los nombres visibles con `*`. Comprueba si aparece `.oculto` y explica por qué.

## Recordatorio

- `*` coincide con cero o más caracteres.
- `?` coincide con exactamente un carácter.
- `[abc]` coincide con un carácter de la lista; `[3-8]` coincide con un carácter del rango.
- Los patrones normales no incluyen nombres ocultos que empiezan por `.`. Para encontrarlos, el patrón debe empezar explícitamente por un punto.