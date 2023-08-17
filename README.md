
----

```Ruby
By: Desmon  
Github: https://github.com/desmonHak
Tags: #Reversing #Assemblyx86_intel #C #CTF #Linux #32bits
```

Description: 
    Simple CTF de reversing, usted puede compilar el reto con lo siguiente;
```bash
 gcc -O0 -masm=intel -static  -z execstack -m32  -ggdb -no-pie -fno-stack-protector poorboy.c -o poorboy.elf
```

----

Descripcion de las flags usadas:
```bash
 -O0                  = cero optimizaciones
 -static              = codigo+lib statico (no usado)
 -masm=intel          = ensamblador con sitaxis intel 
 -z execstack         = stack ejecutable
 -m32                 = codigo de 32bits
 -ggdb                = con informacion de depuracion para gdb (no usado)
 -fno-stack-protector = sin proteciones de stack
```

Para obtener la solucion compile añadiendo ```-D __SEE_ALL_FLAG__``` a lo anterior y vuelva a ejecutar el comando. Otra manera es descomprimir flags.zip donde se encuentra las soluciones y el codigo del programa. Ademas de una version del mismo ya compilada para dar las soluciones directamente

----

Para comprobar los hash's obtenidos use ```solution.elf```:
```bash
┌──(desmon㉿DESKTOP-1GKF8CS)-[/mnt/c/Users/Desmon0x90/Desktop/Reto_ReverC_ASM]
└─$ ./solution.elf
Modo de uso:
./solution.elf <1/2/3/4> <hash md5 obtenido>
<1/2/3/4> es el numeo del hash obtenido, 1 para hash1 y consecutivamente.
<hash md5 obtenido> sera el hash que usted obtuvo.
```

----
