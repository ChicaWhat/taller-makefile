# Define el nombre del ejecutable
NAME=program

# Define las flags del compilador
COMPILER=cc
CFLAGS=-Wall -Wextra -Werror

# Lista de archivos fuente del proyecto
SRC= src/main.c src/utils.c

# Regla principal que compila el programa
all: $(NAME)

$(NAME): 
	$(COMPILER) $(CFLAGS) $(SRC) -o $(NAME)

# Elimina el archivo ejecutable
clean:
	@rm $(NAME)

fclean: clean
	
# Ejecuta clean y luego all para recompilar todo
re: fclean all
	
# Ejecuta el programa
run: re
	@./$(NAME)
# Declara las reglas que no generan archivos
.PHONY: all clean fclean re run
