# BottlerOS

BottlerOS es un sistema operativo...

## Table de contenidos
* [Requisitos](#requisitos)
* [Compilación](#compilación)
* [Ejecución](#ejecución)
* [Testeos](#tests)

## Requisitos <a name="requisitos"></a>

Debe instalar nasm, qemu, gcc, make. Estos se encuentra disponibles en el repositorio de la vasta mayoría de distribuciones de Linux/macOS.

Debian/Ubuntu: `apt install nasm qemu gcc make`\
macOS (con [homebrew](https://brew.sh/)): `brew install nasm qemu gcc make`

Si tiene otra distribución consulte cómo hacerlo.

## Compilación <a name="compilación"></a>

Para compilar todos los archivos se debe ejecutar el script `build.sh` (desde la carpeta raíz del proyecto). Note que usted podrá pasarle como argumento `buddy` si desea compilar con este memory manager (por defecto no compilará con este).

```bash
./build.sh
```

## Ejecución <a name="ejecución"></a>

Ahora, usted podrá ejecutar BottlerOS haciendo:

```bash
./run.sh
```

Si, en su defecto, usted quiere correr el OS desde windows lo podrá hacer con:

```bash
./run.bat
```

## Testeos <a name="tests"></a>

En orden de realizar un análisis estático del sistema usted debe tener instalado [cppcheck](http://cppcheck.net/) y [pvs-studio](https://pvs-studio.com/). Luego, puede correrlos con:

```bash
make test
```

Por último, si quiere hacer un análisis dinámico (usando [valgrind](https://valgrind.org/)) debe ejecutar ...

# Autores
- Barmasch, Juan Martín (61033)
- Bellver, Ezequiel (61268)
- Lo Coco, Santiago (61301)