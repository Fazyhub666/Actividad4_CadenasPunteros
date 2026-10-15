# CADENASPUNTEROS

Programa en C++ que implementa un control de acceso por edad operando directamente sobre la memoria RAM mediante punteros y desreferenciación.

## Descripción

El programa declara una variable entera `edad` y un puntero `p` que guarda su dirección de memoria (`int* p = &edad;`). Luego pide la edad al usuario y la guarda con `cin >> *p;`, escribiendo directamente en el casillero de memoria de `edad`. Si el valor es 18 o más, muestra **ACCESO APROBADO**; si no, **ACCESO RECHAZADO**. En ambos casos informa la edad registrada y la dirección física en RAM en formato hexadecimal.

## Conceptos aplicados

- Memoria RAM y direcciones hexadecimales
- Puntero (`int* p`)
- Operador de dirección (`&`)
- Desreferenciación (`*`)
- Estructura condicional `if / else`

## Estructura del proyecto

```
cadenaspunteros/
├── .gitignore
├── LICENSE
├── README.md
├── docs/
│   └── InformeProyectoCADENASPUNTEROS.pdf
├── src/
│   └── main.cpp
└── capturas/
    ├── ejecucion_punteros.png
    └── esquema_ram.png
```

## Requisitos

- Compilador g++ (MinGW / MSYS2) o, en su defecto, OnlineGDB
- Visual Studio Code (opcional)

## Compilación y ejecución (PowerShell, Windows 10/11)

Desde la raíz del proyecto:

```
g++ src/main.cpp -o src/cadenaspunteros.exe
.\src\cadenaspunteros.exe
```

## Ejemplo de uso

```
=> Ingrese su edad: 20

--- ANALIZANDO ACCESO SEGURO EN MEMORIA ---
[ACCESO APROBADO] El usuario es mayor de edad.
Edad registrada: 20 anos.
Direccion fisica en RAM Hexadecimal: 0x61fe1c
```

La dirección hexadecimal cambia según el equipo y la ejecución.

## Autor

[Nombre y Apellido]
E.E.S.T. N.º 1 "Eduardo Ader", Vicente López
Laboratorio de Programación (LPR), 5.º año, 2026
