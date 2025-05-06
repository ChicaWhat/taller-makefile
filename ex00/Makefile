# Crear una variable
NAME=hola

# Crear una regla para que ejecute un hello world
run: 
	echo $(NAME)

# Crear un directorio y un archivo
create:
	mkdir folder
	touch folder/new-file
# Establecer el contenido de un archivo (sobreescribir)
set:
	echo "new content" > folder/new-file

# Añadir contenido a un archivo (sin sobreescribir)
append:
	echo "new content" >> folder/new-file

# Mostrar el contenido de un archivo
show:
	cat folder/new-file

# Limpiar los archivos y directorios creados
rm:
	rm -rf folder

# Ejecutar clean y luego create
re:
	rm create

# Declarar PHONY
.PHONY: create set append show rm re
