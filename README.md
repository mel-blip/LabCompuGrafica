# LabCompuGrafica

Prácticas del **Laboratorio de Computación Gráfica e Interacción Humano-Computadora** (CGIHC), Grupo 9.

Todas las prácticas están desarrolladas en C++ con OpenGL, sobre un mismo proyecto de Visual Studio (`configBasicaMelissa`). Cada práctica está guardada en su propio commit y marcada con un tag, así que se puede abrir cualquiera de ellas en el estado exacto en que se entregó.

## Prácticas

| Tag | Práctica | Archivo principal |
|---|---|---|
| `Practica1` | Introducción a OpenGL | `Main_Dibujo2D.cpp` |
| `Practica2` | Proyecciones y Puertos de vista. Transformaciones Geométricas | `Main_P3.cpp` |
| `Practica3` | Modelado Geométrico | `Main_Modelado.cpp` |
| `Practica4` | Modelado Jerárquico | `Modelado_Jerarquico.cpp` |
| `Practica5` | Carga de modelos y cámara sintética | `Carga de Modelos.cpp` |
| `Practica6` | Texturizado | `Texturizado.cpp` |
| `Practica7` | Iluminación I | `Iluminacion.cpp` |
| `Practica8` | Iluminación II | `fuentesDeLuz.cpp` |
| `Practica9` | Animación | `Animación_Básica.cpp` y `Maquina de estados.cpp` |
| `Practica10` | KeyFrames | `KeyFrames.cpp` |

## Requisitos

- **Visual Studio 2022** con la carga de trabajo *Desarrollo para el escritorio con C++*.
- La carpeta **`External Libraries`** (no se incluye en el repositorio). Debe colocarse junto a `configBasicaMelissa.sln` con esta estructura:

```
LabCompuGrafica/
├── configBasicaMelissa.sln
├── External Libraries/
│   ├── GLEW/      (include y lib/Release/Win32)
│   ├── GLFW/      (include y lib-vc2015, 32 bits)
│   ├── GLM/
│   ├── assimp/    (include y lib)
│   └── SOIL2/     (lib)
└── configBasicaMelissa/
```

## Cómo compilar

1. Abrir `configBasicaMelissa.sln` en Visual Studio.
2. Seleccionar la configuración **Debug** y la plataforma **x86**.
3. **Compilar → Recompilar solución** y ejecutar.

> Todas las librerías son de 32 bits, por lo que el proyecto debe compilarse en **x86**.

## Cómo abrir una práctica anterior

```bash
git clone https://github.com/mel-blip/LabCompuGrafica.git
cd LabCompuGrafica

# Ir a una práctica (por ejemplo, la 3)
git checkout Practica3

# Regresar a la versión más reciente
git checkout master
```

Después de cambiar de práctica, conviene usar **Recompilar solución** para no ejecutar el binario de la práctica anterior. También se puede descargar cualquier práctica como `.zip` desde la pestaña **Tags** de GitHub.

## Notas

- Los archivos `.cpp` de prácticas anteriores se conservan en la carpeta, pero solo el de la práctica correspondiente está agregado al proyecto en cada commit.
- En la **Práctica 9** hay dos ejercicios. Para ejecutar el otro, se quita del proyecto el `.cpp` actual y se agrega el otro desde el Explorador de soluciones.
- Las animaciones avanzan una cantidad fija por cuadro, por lo que su velocidad puede variar según la computadora.

## Autora

**mel-blip**
