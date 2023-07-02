# **MANUAL TÉCNICO**

## **Descripción general**

Para la presente actividad se le solicita el desarrollo de un juego sencillo empleando las características gráficas que brinda DOS y el conjunto de interrupciones que este provee.

Junto a este juego, se desarrollará la interfaz que permitirá manejarlo, el manejo de puntajes más altos, carga de niveles y configuración de controles.

El juego a desarrollar es el juego japonés Sokoban, en el cual el jugador tiene como principal objetivo empujar una serie de cajas hasta conseguir que éstas se ubiquen en ciertas posiciones. Cuando el jugador consigue lo anterior se le permite avanzar de nivel y acumular más puntos.

También se contabilizará el tiempo del jugador en cada partida, dato que también será asociado a la puntuación obtenida por el jugador.

## **Requisitos minimos del sistema**
---

1. **Sistema operativo:** El proyecto está diseñado para ejecutarse en DOSBox, un emulador que permite ejecutar aplicaciones DOS en sistemas operativos modernos como Windows, macOS o Linux. Asegúrate de tener instalado DOSBox en tu sistema antes de continuar.

2. **Versión de DOSBox:** Se recomienda utilizar la versión X.X.X de DOSBox para garantizar la compatibilidad y el rendimiento óptimo con el proyecto. Puedes descargar la versión recomendada desde el sitio oficial de DOSBox (www.dosbox.com) o cualquier otro repositorio confiable.

3. **Especificaciones de hardware:**

    - Procesador: Se recomienda un procesador de al menos X MHz para garantizar un rendimiento fluido del proyecto.
    - Memoria RAM: Se requieren al menos Y MB de memoria RAM para ejecutar el proyecto sin problemas.
    - Espacio en disco: Asegúrate de tener Z MB de espacio libre en disco para la instalación y funcionamiento del proyecto.

4. **Configuraciones adicionales:** Antes de ejecutar el proyecto, asegúrate de ajustar las siguientes configuraciones en DOSBox para un funcionamiento óptimo:

    - Asignación de memoria: Si el proyecto requiere una cantidad específica de memoria, asegúrate de configurar DOSBox para asignar la cantidad adecuada de memoria al inicio.
    - Velocidad de emulación: Si el proyecto tiene requisitos de velocidad específicos, ajusta la velocidad de emulación en DOSBox para que coincida con los requisitos del proyecto.

## **Tecnologías Utilizadas**
---

En el desarrollo de este proyecto en ensamblador utilizando DOSBox, se utilizaron diversas tecnologías y herramientas. A continuación, se detallan las principales tecnologías utilizadas:

* Ensamblador: El ensamblador es un lenguaje de programación de bajo nivel que se utiliza para escribir código directamente ejecutable por el procesador de la computadora. A diferencia de los lenguajes de programación de alto nivel, el ensamblador proporciona un control preciso sobre el hardware y las instrucciones del procesador. Permite escribir programas eficientes y optimizados para tareas específicas. En este proyecto, el ensamblador se utilizó para aprovechar al máximo las capacidades del hardware y desarrollar un programa de alto rendimiento.

* DOSBox: DOSBox es un emulador diseñado para ejecutar aplicaciones diseñadas para el sistema operativo DOS en sistemas operativos modernos. Proporciona una plataforma virtual que emula el entorno de ejecución de DOS. DOSBox emula componentes clave de la arquitectura de hardware, como la CPU, el sistema de archivos y el entorno de memoria, lo que permite ejecutar programas antiguos sin tener que usar un sistema operativo DOS físico. En este proyecto, DOSBox se utilizó para crear un entorno DOS virtual en el que se pudiera ejecutar y probar el programa desarrollado en ensamblador.

* Editor de texto: Para escribir y editar el código fuente en ensamblador, se utilizó un editor de texto compatible con el formato de archivos de código ensamblador, como NASM (Netwide Assembler) o TASM (Turbo Assembler). Estos editores de texto están diseñados específicamente para trabajar con lenguajes de bajo nivel y proporcionan características que facilitan la escritura y edición del código, como el resaltado de sintaxis, la numeración de líneas, la indentación automática y la verificación de errores. Además, ofrecen funciones de búsqueda y reemplazo que ayudan a trabajar de manera eficiente y organizada con el código fuente del proyecto.

* El sistema operativo DOS (Disk Operating System) es un sistema operativo de línea de comandos que fue ampliamente utilizado en las primeras computadoras personales. Proporciona una interfaz de usuario basada en comandos a través de la cual los programas pueden acceder a los recursos del sistema, como el sistema de archivos, la memoria y los dispositivos de entrada y salida. En este proyecto, el código fuente del programa se desarrolló teniendo en cuenta las limitaciones y características específicas del sistema operativo DOS. Se utilizaron llamadas al sistema operativo DOS y funciones de interrupción para interactuar con el entorno y los servicios proporcionados por el sistema operativo.

Cada una de estas tecnologías desempeña un papel crucial en el desarrollo y la ejecución del proyecto en ensamblador. El ensamblador permite un control detallado sobre el hardware y las instrucciones del procesador, DOSBox proporciona un entorno virtual para ejecutar el programa en un sistema DOS simulado, el editor de texto facilita la escritura y edición del código fuente de manera eficiente, y el sistema operativo DOS es el entorno objetivo en el que se ejecuta el programa y se interactúa con los recursos del sistema.

## **Instalación**
---
Para poder ejecutar el proyecto en ensamblador utilizando DOSBox, es necesario seguir los siguientes pasos de instalación:

1. **Requisitos del Sistema:** Asegúrate de que tu sistema cumpla con los requisitos mínimos para ejecutar DOSBox correctamente. Estos requisitos pueden incluir un sistema operativo compatible (como Windows, macOS o Linux), una cantidad mínima de memoria RAM y una velocidad de CPU adecuada.

2. **Descarga de DOSBox:** Visita el sitio web oficial de DOSBox en www.dosbox.com y busca la sección de descargas. Allí encontrarás las versiones más recientes de DOSBox disponibles para diferentes sistemas operativos. Descarga la versión adecuada para tu sistema y guárdala en una ubicación conveniente.

3. **Instalación de DOSBox:** Ejecuta el archivo de instalación de DOSBox que descargaste y sigue las instrucciones del asistente de instalación. Durante el proceso de instalación, se te pedirá que elijas una ubicación de instalación y que aceptes los términos y condiciones de uso.

4. **Configuración de DOSBox:** Después de la instalación, abre DOSBox. Se te presentará una ventana de línea de comandos similar a la de un sistema MS-DOS. Antes de ejecutar tu proyecto en ensamblador, es necesario configurar algunos parámetros.

    - **Montar unidades virtuales:** Utiliza el comando mount para asignar una unidad virtual en DOSBox. Por ejemplo, si tu proyecto utiliza un archivo de imagen de disco llamado "project.img", puedes usar el comando mount c path/to/project.img -t floppy para asignarla como unidad C en DOSBox.

    - **Configuración de teclado:** Si necesitas ajustar la configuración del teclado, puedes usar el comando keyb seguido del código del idioma correspondiente. Por ejemplo, keyb us para el idioma inglés.

    - **Otros ajustes:** Puedes explorar las opciones de configuración adicionales de DOSBox, como la velocidad de emulación, el tamaño de la ventana y el mapeo de teclas, mediante el archivo de configuración "dosbox.conf" ubicado en la carpeta de instalación de DOSBox.

5. **Carga y ejecución del proyecto:** Una vez que DOSBox esté configurado, puedes cargar y ejecutar tu proyecto en ensamblador utilizando los comandos y procedimientos específicos del ensamblador que estés utilizando. Esto puede implicar compilar tu código fuente y crear un archivo ejecutable que luego se pueda ejecutar dentro de DOSBox.

6. **Pruebas y verificación:** Una vez que el proyecto esté en ejecución, realiza pruebas exhaustivas para asegurarte de que funcione correctamente dentro del entorno DOSBox. Verifica que las funcionalidades del proyecto se comporten según lo esperado y soluciona cualquier problema o error que encuentres.

## **Resumen - Macros Utilizadas**
---

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **MoverPuntero**    |   Se encarga de mover el cursos a cierta posicion de la pantalla    |

```js
;; Mueve el cursor a una posición
MoverPuntero MACRO xpos,ypos
    mov AH,02h  ; establece la posición del cursor
    mov BH,00h  ; es el numero de la pag.
    mov DH,ypos ; fila
    mov DL,xpos ; col
    int 10h
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **TomarPosicionCursor**    |   Se encarga de tomar la posicion del cursor, y asi verificar las coordenadas de este    |

```js
TomarPosicionCursor MACRO
    mov AH,03h  ; toma las posiciones del cursor; DH: row , DL: col
    mov BH,0h   ; en el modo grafico
    int 10h
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **ImprimirTextoEspecifico**    |   Imprime una porción de texto en una posicion especifica de la pantalla    |

```js
ImprimirTextoEspecifico MACRO xpos, ypos, stringbuffer, color
    push SI
    MoverPuntero xpos,ypos
    lea SI,stringbuffer 
    mov BL,color
    call Imprimir_Str 
    pop SI
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **PonerSprite**    |   Coloca el sprite (lo que viene siendo la figura en pixeles de lo que se quiere pintar en pantalla) en una fila y columna especifico    |

```js
PonerSprite MACRO sprite,col,row
    lea SI, sprite
    mov DH,col
    mov DL,row
    call Renderizar_sprite
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **LimpiarBuffer**    |   Simplemente limpiar el buffer que ha sido ingresado    |

```js
LimpiarBuffer MACRO buffer,len_buff
    push DI
    mov DI, offset buffer
    mov AL,0
    mov CX,len_buff
    rep stosb
    pop DI 
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **LimpiarBufferJuego**    |   Simplemente limpiar el buffer que ha sido ingresado o utilizado dentro del juego   |

```js
LimpiarBufferJuego MACRO buffer,len_buff
    push DI
    mov DI, offset buffer
    mov AL,0FFh
    mov CX,len_buff
    rep stosb
    pop DI 
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **BufferAtoi**    |   Esta macro hace el parseo de una cadena string a un valor numérico  |

```js
BufferAtoi MACRO buffer_str, buffer_num
    push BX
    xor SI,SI
    xor AH,AH
    lea SI, buffer_str
    call atoi
    mov BH,00h
    mov [buffer_num],BL
    pop BX
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **BufferItoa**    |   Esta macro hace el parseo de un valor numérico a una cadena de caracteres o string  |

```js
BufferItoa MACRO buffer1,buffer2
    xor AX,AX
    mov AX,[buffer1]
    mov BX,offset buffer2
    call itoa
    mov AX,[buffer1]
    call padCeroding
    AnadirBufferTMP buffer2,20h,0
    LimpiarBuffer buffer2,20h
    lea DI,buffer2
    AnadirBufferTMP buffer_g,20h,0 
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **ImprimirString**    |   Basicamente hace la impresion de una cadena o string, es por ello que recibe el buffer donde se encuentra dicha cadena  |

```js
ImprimirString MACRO buffer
    mov SI, offset buffer
    call Imprimir_Str
ENDM
```

| ***Nombre*** | ***Descripción*** |
|--------------|--------------|
|   **RenderizarPos**    |   Esta macro, hace la renderizacion de las pociciones dentro del juego, para volver a hacer alguna acción dentro de este |

```js
RenderizarPos MACRO thingX,thingY,skip
    xor SI,SI
    mov x_temportal,00h
    mov y_temporal,00h

    lea SI,thingX
    add SI,skip
    lodsb
    mov [x_temportal],AL
    cmp x_temportal,0FFh
    je Finalizar_suelo

    xor SI,SI
    lea SI,thingY
    add SI,skip
    lodsb
    mov [y_temporal],AL
ENDM
```


## **Subrutinas Importantes**
---

- ### **Subrutina Renderizar_sprite**

```js
;; SI:Sprite DH:posX (columna) DL:posY (linea) 
;; Renderiza el sprite en una posición Columna,Fila (40x25)
Renderizar_sprite:		
    push ES
    push DS
	mov AX,0A000h
	mov ES,AX
	mov AX,@CODE
	mov DS,AX
	
	push DX	
    mov AX,08h
    mul DH
    mov DI,AX
        
    mov AX,0A00h
    mov BX,00h
    add BL,DL
    mul BX
    add DI,AX

	pop DX
	
	mov CL,08h			                                                ; Altura 8px
DibujarY:
	push DI
    mov CH,08h		                                                    ; Longitud 8px
DibujarX:				
    mov AL,DS:[SI]

    ;; xor AL,ES:[DI] --> Si se imprime el mismo sprite en el mismo lugar, se "borra"
    mov ES:[DI],AL
    inc SI
    inc DI
    dec CH
    jnz DibujarX                                                        ; Siguiente pixel horizontal 
	pop DI
	add DI,0140h			                                            ; Ir una línea hacia abajo (320px)
	inc BL
	dec CL
	jnz DibujarY
    pop ES
    pop DS
	ret	
```

- ### **Subrutina cadenaAnum**

```js
;;;;;;;;;;          Subrutina cadenaAnum          ;;;;;;;;;;
;; ENTRADAS
;;        o AX -> numero a convertir
;; SALIDAS
;;        o [numero] -> numero convertido en cadena
cadenaAnum:
    mov AX, 0000    ; inicializar la salida
    mov CX, 0005    ; inicializar contador
		
    seguir_convirtiendo:
        mov BL, [DI]
        cmp BL, 00
        je retorno_cadenaAnum
        sub BL, 30      ; BL es el valor numérico del caracter
        mov DX, 000a
        mul DX          ; AX * DX -> DX:AX
        mov BH, 00
        add AX, BX 
        inc DI          ; puntero en la cadena
        loop seguir_convirtiendo
        retorno_cadenaAnum:
            ret
```

- ### **Subrutina numAcadena**

```js
;;;;;;;;;;          Subrutina cadenaAnum          ;;;;;;;;;;
;; ENTRADAS
;;        o AX -> número a convertir
;; SALIDAS
;;        o [numero] -> numero convertido en cadena
numAcadena:
    
    mov CX, 0005
    mov DI, offset numero

    ciclo_poner30s:
        mov BL, 30
        mov [DI], BL
        inc DI
        loop ciclo_poner30s
        ;; tenemos '0' en toda la cadena

        mov CX, AX                              ; inicializar contador
        mov DI, offset numero
        add DI, 0004
		
        ciclo_convertirAcadena:
            mov BL, [DI]
            inc BL
            mov [DI], BL
            cmp BL, 3a
            je aumentar_siguiente_digito_primera_vez
            loop ciclo_convertirAcadena
            jmp retorno_convertirAcadena

            aumentar_siguiente_digito_primera_vez:
                push DI

                aumentar_siguiente_digito:
                    mov BL, 30     ; poner en '0' el actual
                    mov [DI], BL
                    dec DI         ; puntero a la cadena
                    mov BL, [DI]
                    inc BL
                    mov [DI], BL
                    cmp BL, 3a
                    je aumentar_siguiente_digito
                    pop DI         ; se recupera DI
                    loop ciclo_convertirAcadena

    retorno_convertirAcadena:
    ret
```

- ### **Subrutina Analizar_nivel**

```js
;; -> AH  00 -> LV.00  01 -> LV.01 02 -> LV.10 03 -> Arbitrario (?)
Analizar_nivel:
    call Limpiar_assets_nivel 
    cmp AH,00h
    je Nivel_uno
    cmp AH,01h
    je Nivel_dos
    cmp AH,02h
    je Nivel_tres
    cmp AH,03h
    je Nivel_arbitrario
 
    Nivel_uno:    
        mov DX, offset nombre_nivel1
        jmp Cargar_archivo

    Nivel_dos:
        mov DX, offset nombre_nivel2
        jmp Cargar_archivo

    Nivel_tres:
        mov DX, offset nombre_nivel3
        jmp Cargar_archivo

    Nivel_arbitrario:
        lea DX, nombre_nivelA
        jmp Cargar_archivo

    Cargar_archivo:
        mov AL, 2
        mov AH, 3Dh
        int 21h
        mov [handle_nivel], AX
        mov BX,[handle_nivel]
        jc menu_principal                                                   ; el archivo a abrir no fue encontrado
        call Iniciar_video
    Leer_caracter:
        LimpiarBuffer char_temporal,0a
        mov AH,3Fh
        mov CX,01h
        mov DX,offset char_temporal
        int 21h
        jc Finalizar_lectura                                                ; carry flag si hay error, no parece funcionar como yo esperaba xd
        cmp AX,0000h                                                        ; si no lee nada
        je Finalizar_lectura

        call Saltar_espacio
        cmp char_temporal,'c' ; c aja
        je Leer_caja
        cmp char_temporal,'j' ; j ugador
        je Leer_jugador
        cmp char_temporal,'p' ; p ared
        je Leer_pared
        cmp char_temporal,'o' ; o bjetivo
        je Leer_objetivo
        cmp char_temporal,'s' ; s uelo
        je Leer_suelo
        ret
```

- ### **Subrutina Renderizar_mapa**

```js
Renderizar_mapa:
    call Iniciar_video                                          ; usandolo como clearsecreen
    call Renderizar_pared
    call Renderizar_suelo
    call Renderizar_objetivo
    call Renderizar_caja
    call Renderizar_jugador
    ImprimirTextoEspecifico 00h,LINEA_BOTON,datos_pantalla,COLOR_GRIS 
    ret
```

- ### **Subrutina Renderizar_suelo**

```js
Renderizar_suelo:
    mov counter_g,0000h                                         ; contador para imprimir SI 
    Renderizar_sueloTile:

    ; posx_suelo , posy_suelo
    RenderizarPos posx_suelo,posy_suelo,counter_g

    xor AX,AX
    xor SI,SI
    lea SI,suelo
    mov DH,[x_temportal]
    mov DL,[y_temporal]
    call Renderizar_sprite

    inc counter_g
    jmp Renderizar_sueloTile
    Finalizar_suelo:
        mov counter_g,0000h
        ret
```

- ### **Subrutina Renderizar_pared**

```js
Renderizar_pared:
    mov counter_g,0000h                                         ; contador para imprimir SI 
    Renderizar_pared_tile:

    ; posx_pared , posy_pared
    RenderizarPos posx_pared,posy_pared,counter_g
    
    xor AX,AX
    xor SI,SI
    lea SI,pared
    mov DH,[x_temportal]
    mov DL,[y_temporal]
    call Renderizar_sprite

    add counter_g,0001h
    jmp Renderizar_pared_tile
    Finalizar_pared:
        mov counter_g,0000h
        ret
```

- ### **Subrutina Renderizar_caja**

```js
Renderizar_caja:
    mov counter_g,0000h                                         ; contador para imprimir SI 
    Renderizar_caja_tile:

    ; posx_pared , posy_pared
    RenderizarPos posx_caja,posy_caja,counter_g
    
    xor AX,AX
    xor SI,SI
    lea SI,caja
    mov DH,[x_temportal]
    mov DL,[y_temporal]
    call Renderizar_sprite

    add counter_g,0001h
    jmp Renderizar_caja_tile
    Finalizar_caja:
        mov counter_g,0000h
        ret
```

- ### **Subrutina Renderizar_objetivo**

```js
Renderizar_objetivo:
    mov counter_g,0000h                                         ; contador para imprimir SI 
    Renderizar_obj_tile:

    ; posx_pared , posy_pared
    RenderizarPos posx_obj,posy_obj,counter_g
    
    xor AX,AX
    xor SI,SI
    lea SI,objetivo
    mov DH,[x_temportal]
    mov DL,[y_temporal]
    call Renderizar_sprite

    add counter_g,0001h
    jmp Renderizar_obj_tile
    Finalizar_objeto:
        mov counter_g,0000h
        ret
```

- ### **Subrutina Renderizar_jugador**

```js
Renderizar_jugador:
    lea SI,jugador
    mov DH,[posx_jugador]
    mov DL,[posy_jugador]
    mov x_temportalP,DH
    mov y_temporalP,DL
    call Renderizar_sprite
    ret
```

## **Resumen - Variables**
---

- ### **Definicíon de los sprites utilizados para los graficos del juego**
    
    ```js
    pared:    
        db 49, 48, 32, 1c, 1c, 1c, 49, 49
        db 48, 32, 1c, 49, 49, 49, 48, 32
        db 48, 78, 49, 48, 48, 32, 31, 31
        db 32, 1c, 49, 48, 32, 31, 31, 78
        db 31, 1c, 48, 32, 31, 78, 1c, 1c
        db 1c, 49, 48, 78, 1c, 1c, 49, 49
        db 1c, 78, 78, 49, 49, 48, 48, 32
        db 49, 1c, 49, 48, 32, 32, 31, 1c

    caja:
        db 42, 42, 42, 00, 42, 42, 42, 42
        db 42, 42, 00, 35, 00, 42, 42, 42
        db 42, 42, 00, 35, 00, 42, 42, 42
        db 42, 00, 35, 21, 21, 00, 42, 42
        db 42, 00, 0f, 35, 21, 00, 42, 42
        db 42, 00, 0f, 35, 21, 00, 42, 42
        db 42, 42, 00, 0f, 00, 42, 42, 42
        db 42, 42, 42, 00, 42, 42, 42, 42

    suelo:
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42
        db 42, 42, 42, 42, 42, 42, 42, 42

    objetivo:
        db 42,42,00,00,00,00,42,42
        db 42,00,1b,1b,1b,50,00,42
        db 00,1b,17,17,1b,1b,50,00
        db 00,00,00,17,1b,00,00,00
        db 00,0f,1a,00,00,1a,1a,00
        db 42,00,1a,0f,1a,1c,00,42
        db 42,00,1a,0f,1a,1a,00,42
        db 42,42,00,00,00,00,42,42

    jugador:
        db 42, 42, 04, 04, 04, 42, 42, 42 
        db 42, 04, 0E, 0E, 0E, 04, 42, 42 
        db 42, 42, 04, 04, 04, 42, 42, 42 
        db 42, 42, 42, 0A, 42, 42, 42, 42 
        db 42, 42, 02, 0A, 02, 42, 42, 42 
        db 42, 42, 42, 0A, 42, 42, 42, 42 
        db 42, 06, 06, 06, 06, 06, 42, 42 
        db 42, 42, 06, 06, 06, 42, 42, 42 
    ```

- ### **Constantes o variables para los colores**

    ```js
    COLOR_BLANCO        EQU 0Fh
    COLOR_GRIS          EQU 08h
    COLOR_DCYAN         EQU 03h
    COLOR_LCYAN         EQU 0Bh
    COLOR_LROJO         EQU 0Ch
    ```

- ### **Posiciones de la flecha**

    ```js
    POS_INICIAR         EQU 08h
    POS_CARGAR          EQU 0Ah
    POS_CONF            EQU 0Ch
    POS_PUNTOS          EQU 0Eh
    POS_SALIR           EQU 10h

    LINEA_BOTON         EQU 18h

    POS_CONTADOR        EQU 0Ah
    POS_LEAV            EQU 0Eh
    ```
- ### **Teclas del menu principal**

    ```js
    TECLA_F1            EQU 3Bh
    CLAVE_ARRIBA        EQU 48h
    CLAVE_ABAJO         EQU 50h
    TECLA_F2            EQU 3Ch
    ```

- ### **Variables para los movimientos e items dentro del juego, manipulacion, coordenadas, objetos, etc.**

    ```js
    DESP_U  EQU 01h
    DESP_D  EQU 02h 
    DESP_L  EQU 03h
    DESP_R  EQU 04h
    V_DESP  db 0
    
    iniciar_juego       db "INICIAR JUEGO",0
    cargar_nivel        db "CARGAR NIVEL",0
    config              db "CONFIGURACION",0
    puntajes            db "PUNTAJES ALTOS",0
    salir               db "SALIR",0
    datos               db "Anthony Samuel Zea Herrera - 202104782",0
    datos_pantalla      db "ASZH - 20214782",0
    vacio               db " ",0

    msg_ganaste         db "GANASTE!",0
    msg_continuar       db "CONTINUAR",0
  
    arrow               db 10h,0
    ```


- ### **Controles por defecto**

    ```js
    tecla_arriba        db 48h
    tecla_abajo         db 50h
    tecla_derecha       db 4Dh
    tecla_izquierda     db 4Bh
    ```

- ### **Variables para el manejo de archivos (niveles)**

    ```js
    nombre_nivel1   db "NIV.00",0
    nombre_nivel2   db "NIV.01",0
    nombre_nivel3   db "NIV.10",0
    nombre_nivelA   db 20h dup (0),0
    KbIn_nivel      db 21h,20h,22h dup (0),0
    prompt_nivel    db "Ingrese el nombre de archivo:",0
    handle_nivel    dw 0000
    counter_g       dw 0000
    counter_g2      dw 0000
    buffer_g        db 20h dup(0),0
    buffer_g2       db 20h dup(0),0
    ```

- ### **Variables para posiciones de itemas en el mapa del juego**

    ```js
    ;; Coordenadas en columnas y lineas -> 30 cajas - 30 objetivos
    posx_caja       db 1Eh  dup (0FFh),0FFh
    posy_caja       db 1Eh  dup (0FFh),0FFh
    posx_obj        db 1Eh  dup (0FFh),0FFh
    posy_obj        db 1Eh  dup (0FFh),0FFh

    ;; Suelo y paredes
    posx_pared      db 0FFh dup (0FFh),0FFh
    posy_pared      db 0FFh dup (0FFh),0FFh
    posx_suelo      db 0FFh dup (0FFh),0FFh
    posy_suelo      db 0FFh dup (0FFh),0FFh

    ;; Contador del número de objetos en el mapa
    cont_cajas      db 0,0
    cont_obj        db 0,0
    cont_pared      db 0,0
    cont_suelo      db 0,0
    
    ;; X-Y del jugador
    posx_jugador    db 0
    posy_jugador    db 0
    
    ;; Guarda el objeto en donde esta el jugador
    over_jugador    db 0,0

    ;; Variables temporales para las coordenadas
    x_temportal         db 0,0
    y_temporal          db 0,0
    x_temportalP        db 0
    y_temporalP         db 0

    x_temportalB        db 0
    y_temporalB         db 0
    
    char_temporal       db 0a dup (0),0

    curr_nivel      db 0
    curr_scr        dw 0000
    
    timer           db 0
    segundos        db 0
    minutos         db 0
    horas           db 0
    segundos2b      dw 0000
    minutos2b       dw 0000
    horas2b         dw 0000
    padCero         db "0",0
    pad2            db "00",0
    pad3            db "000",0
    puntos          db ":",0
    ```

## **Limitaciones y mejores futuras**
---

En esta sección, se describen las limitaciones conocidas del proyecto en ensamblador, así como las posibles mejoras y funcionalidades adicionales que podrían implementarse en versiones futuras.

- Limitaciones Actuales:

    * Rendimiento limitado en ciertos escenarios de carga de datos masivos.
    Requiere una configuración específica de hardware y sistema operativo.
    * No es compatible con sistemas operativos modernos.
    Ausencia de manejo de errores y recuperación en casos de fallos inesperados.
    * La interfaz de usuario actual puede resultar poco intuitiva para usuarios no familiarizados con ensamblador.

- Mejoras Futuras:

    * Optimización de algoritmos y estructuras de datos para mejorar el rendimiento en situaciones de carga de datos masivos.
    * Implementación de soporte para sistemas operativos más recientes y ampliación de la compatibilidad de hardware.
    * Incorporación de un sistema de manejo de errores robusto y mecanismos de recuperación ante fallos.
    * Mejora de la interfaz de usuario, incluyendo elementos gráficos y una experiencia más intuitiva.
    * Adición de funcionalidades adicionales, como la capacidad de exportar resultados a formatos comunes, integración con herramientas de depuración y optimización del código ensamblador generado.

- Prioridades y Planificación:

   * Se priorizará la optimización del rendimiento y la compatibilidad con sistemas operativos modernos en las próximas versiones.
    * Las mejoras en la interfaz de usuario y el manejo de errores se abordarán en etapas posteriores del desarrollo.
    * Se establecerá una hoja de ruta con fechas estimadas para cada mejora y se asignarán los recursos necesarios para su implementación.
    * Consideraciones de Retrocompatibilidad:

    *   Se trabajará para garantizar la compatibilidad con proyectos y código existente en futuras actualizaciones.
    * Se proporcionarán instrucciones claras sobre cómo migrar a nuevas versiones y se mantendrá la retrocompatibilidad en la medida de lo posible.

- Solicitudes de Retroalimentación:

    * Se alienta a los usuarios y colaboradores a proporcionar comentarios, informar de problemas y enviar sugerencias de mejora.
    * Se facilitará un canal de comunicación, como un correo electrónico o un foro en línea, para que los usuarios puedan compartir su retroalimentación y contribuir al desarrollo continuo del proyecto.