# Definir el compilador
CC = gcc

# Definir las opciones de compilación
CFLAGS = -Wall -Wextra

# Nombre del archivo fuente
CFILE = main.c

# Nombre del archivo ensamblador
ASMFILE = main.s

# Nombre del archivo objeto
OBJFILE = main.o

# Regla por defecto
all: $(ASMFILE)

# Regla para generar el archivo ensamblador
$(ASMFILE): $(CFILE)
	$(CC) -S $(CFILE) -o $(ASMFILE)

# Regla para compilar el archivo C sin enlazar
compila:	
	$(CC) $(CFLAGS) -c $(CFILE) -o $(OBJFILE)

# Limpiar archivos generados
clean:
	rm -f $(ASMFILE) $(OBJFILE)
