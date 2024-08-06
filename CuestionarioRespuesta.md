### Pirez Tiziano 4to 4ta
# Laboratorio 10 : Particiones de Disco Duro

## 1. ¿Qué es una partición de disco duro?
Una partición de disco duro es una división lógica de un disco físico en secciones independientes que permiten al sistema operativo gestionar y organizar el espacio de almacenamiento de manera eficiente. Cada partición puede funcionar como un disco separado.

## 2. ¿Cuáles son los dos esquemas de particionamiento más conocidos?
Los dos esquemas de particionamiento más conocidos son:
- MBR (Master Boot Record)
- GPT (GUID Partition Table)

## 3. ¿Qué es el espacio sin particionar?
El espacio sin particionar es el área del disco duro que no ha sido asignada a ninguna partición. Este espacio no está disponible para almacenar datos hasta que se crea una nueva partición en él.

## 4. Mencione al menos tres sistemas de archivos y sus características principales.
- **NTFS (New Technology File System):** Utilizado principalmente en sistemas Windows, ofrece soporte para archivos grandes, compresión, cifrado y permisos avanzados.
- **ext4 (Fourth Extended Filesystem):** Utilizado en sistemas Linux, ofrece soporte para grandes volúmenes y archivos, y cuenta con características como journaling y defragmentación en línea.
- **HFS+ (Hierarchical File System Plus):** Utilizado en sistemas macOS, soporta características como la codificación de caracteres Unicode y la gestión eficiente de archivos y carpetas.

## 5. ¿Cómo interpreta un sistema operativo las particiones en un disco duro?
Un sistema operativo interpreta las particiones en un disco duro mediante el uso de una tabla de particiones, que contiene información sobre el tipo, tamaño y ubicación de cada partición. Esta tabla permite al sistema operativo acceder y gestionar cada partición de manera adecuada.

## 6. Describa el esquema de partición MBR.
El esquema de partición MBR (Master Boot Record) es un estándar antiguo que utiliza un sector de arranque de 512 bytes en el primer sector del disco. Este sector contiene el código de arranque y una tabla con información de hasta cuatro particiones primarias. MBR tiene un límite de 2 TB para el tamaño máximo de cada partición.

## 7. Describa el esquema de partición GPT.
El esquema de partición GPT (GUID Partition Table) es un estándar moderno que utiliza identificadores únicos globales (GUID) para cada partición. GPT soporta un número prácticamente ilimitado de particiones y permite tamaños de partición mucho mayores que MBR, superando los 2 TB. Además, incluye redundancia y verificación de integridad de los datos.

## 8. ¿Cuáles son los tipos de particiones en un disco duro con MBR?
En un disco duro con MBR, los tipos de particiones son:
- Particiones primarias
- Particiones extendidas
- Unidades lógicas (dentro de las particiones extendidas)

## 9. ¿Cuál es la principal diferencia entre particiones primarias y extendidas?
La principal diferencia entre particiones primarias y extendidas es que las particiones primarias son las que el sistema operativo puede utilizar directamente para arrancar y almacenar datos, mientras que solo puede haber una partición extendida, la cual puede contener múltiples unidades lógicas, permitiendo superar el límite de cuatro particiones en total.

## 10. Compare el número máximo de particiones en discos MBR y GPT.
- **MBR:** Admite un máximo de cuatro particiones primarias, o tres primarias y una extendida con múltiples unidades lógicas.
- **GPT:** Admite hasta 128 particiones en discos estándar y, en teoría, un número casi ilimitado.

## 11. ¿Cuál es el tamaño máximo de volúmenes admitido por los estilos MBR y GPT?
- **MBR:** Soporta un tamaño máximo de volumen de hasta 2 TB.
- **GPT:** Soporta tamaños de volumen de hasta 9.4 ZB (zettabytes), mucho más allá de los requerimientos actuales.
