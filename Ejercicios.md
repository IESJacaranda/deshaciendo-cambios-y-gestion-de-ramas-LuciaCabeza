1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

cd examen_Lucia
cd deshaciendo-cambios-y-gestion-de-ramas-LuciaCabeza
nano scene-5.txt
allí pegamos el texto que tenemos que incorporar
guardamos el archivo 

2. Añade scene-5.txt al área de preparación.

git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

git commit -m "subiendo texto"

4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

nano scene-5.txt 
modificamos el texto que aparece añadiendo el anterior

5. Devuelve el fichero al estado del último commit.

git reset --hard

6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.

nano scene-3.txt
modificamos el nombre 
guardamos
nano scene-7.txt 
modificamos el nombre
guardamos

7. Añade los ficheros al área de preparación usando un único comando git.

git add scene-3.txt scene-7.txt

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.

nano scene-2.txt
borramos una linea

9. Añade scene-2.txt al área de preparación.

git add scene-2.txt

10. Comprueba el estado del repositorio. 

git status

11. Devuelve scene-2.txt al directorio de trabajo.

git checkout scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.

git commit scene-3.txt scene-7.txt -m "guardar cambios larry"

13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.

git log
te aparecen los commit que has realizado
en este caso el primero que he realizado ha sido 24330a9113ce68509cfb78a62780c3c3e0a16a86

14. Crea una nueva rama llamada **reinventando_hamlet**

git checkout -b reinventando_hamlet
git push origin reinventando_hamlet

15. Cámbiate a dicha rama

al crearla estamos por defecto en ella pero si quisiéramos cambiarnos se usaria 
git checkout reinventando_hamlet

16. Mejora la escena 2 como creas conveniente.

nano scene-2.txt
añadimos texto
guardamos

17. Haz un commit con los cambios con un mensaje adecuado.

git add scene-2.txt
git commit -m "guardando cambios rama"
git push

18. Vuelve a la rama master.

git checkout master

19. Elimina la rama **reinventando_halet**

git branch -d reinventando_halet

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.

git checkout -b nuevo
nano scene-2.txt
modificamos
guardamos

21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.
