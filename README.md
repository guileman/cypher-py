# CYPHER.PY — Learn Python or Die Trying

> Un juego de aprendizaje de Python con estética hacker/ciberpunk.
> Python real en el navegador via Pyodide. Sin servidor. Listo para GitHub Pages.

**[▶ JUGAR AHORA](https://TU_USUARIO.github.io/cypher-py/)**

---

## 🚀 Deploy en GitHub Pages

```bash
git init
git add index.html README.md
git commit -m "feat: CYPHER.PY initial release"
git remote add origin https://github.com/TU_USUARIO/cypher-py.git
git push -u origin main
```

Luego: **Settings → Pages → Source: main branch → Save**

Tu juego estará en: `https://TU_USUARIO.github.io/cypher-py/`

---

## ⚡ Features

- **Python real** en el browser via [Pyodide](https://pyodide.org/) (WebAssembly) — sin servidor
- **33 misiones** organizadas en 8 bloques temáticos
- **Sistema de XP y niveles** con efecto glitch al subir de nivel
- Estética ciberpunk: matrix rain, scanlines CRT, neon glow
- Un solo archivo `index.html` — cero dependencias locales
- **Tab** para indentar, **Ctrl+Enter** para ejecutar código
- Hints desbloqueables por misión

---

## 📋 Misiones

### BLOQUE I — Fundamentos
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-001 | Primera Intrusión | Básico | 25 |
| M-002 | Variables en la Sombra | Básico | 30 |
| M-003 | Tipos de Datos | Básico | 35 |
| M-004 | Loop de Vigilancia | Intermedio | 45 |
| M-005 | Lista Negra | Intermedio | 50 |
| M-006 | Función Encubierta | Intermedio | 55 |
| M-007 | Condicionales del Destino | Intermedio | 50 |
| M-008 | Diccionario del Agente | Intermedio | 60 |
| M-009 | Clase Fantasma | Avanzado | 80 |
| M-010 | Comprensión Total | Avanzado | 75 |
| M-011 | Decorador Oscuro | Avanzado | 90 |
| M-012 | Operación Final | Avanzado | 100 |

### BLOQUE II — Strings y Manipulación
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-013 | Protocolo de Strings | Básico | 30 |
| M-014 | String Formatting | Básico | 35 |
| M-015 | Split & Join | Intermedio | 50 |
| M-016 | Contador de Frecuencias | Intermedio | 55 |

### BLOQUE III — Estructuras y Algoritmos
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-017 | While Loop Infiltrado | Intermedio | 50 |
| M-018 | Filtro de Señales | Intermedio | 60 |
| M-019 | Bubble Sort Clandestino | Avanzado | 80 |
| M-020 | Recursión Profunda | Avanzado | 85 |

### BLOQUE IV — Errores y Módulos
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-021 | Try-Except Blindado | Intermedio | 65 |
| M-022 | Módulo Matemático | Básico | 40 |
| M-023 | Random Infiltrado | Básico | 40 |

### BLOQUE V — Programación Orientada a Objetos
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-024 | Herencia Cibernética | Avanzado | 90 |
| M-025 | Propiedades Ocultas | Avanzado | 85 |

### BLOQUE VI — Funciones Avanzadas
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-026 | Lambda Encubierta | Intermedio | 60 |
| M-027 | Filter & Reduce | Avanzado | 80 |
| M-028 | Generadores Fantasma | Avanzado | 90 |

### BLOQUE VII — Estructuras Avanzadas
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-029 | Set de Intrusos | Intermedio | 55 |
| M-030 | Tuplas Inmutables | Básico | 35 |
| M-031 | Dict Comprehension | Avanzado | 75 |

### BLOQUE VIII — Desafíos Finales
| ID | Nombre | Nivel | XP |
|----|--------|-------|----|
| M-032 | FizzBuzz Cibernético | Intermedio | 65 |
| M-033 | Número Primo | Intermedio | 70 |

**XP Total disponible: 2,320 XP**

---

## 🔧 Cómo agregar misiones

En `index.html`, dentro del array `missions`, agregá un objeto con esta estructura:

```javascript
{
  id: 'M-034',
  name: 'Nombre de la misión',
  diff: 'basico' | 'intermedio' | 'avanzado',
  xp: 50,
  story: 'Narrativa de contexto hacker...',
  objective: 'Descripción del objetivo (HTML permitido: <code>, <strong>)',
  hint: 'Pista en texto plano con \n para saltos de línea',
  starter: '# código inicial\n\n',
  validate: (output) => output.trim() === 'resultado esperado'
}
```

La función `validate` recibe el output del programa como string y debe retornar `true` o `false`.

---

## 📁 Estructura

```
cypher-py/
├── index.html   ← todo el juego (HTML + CSS + JS + misiones)
└── README.md
```

---

## 🛠️ Tecnologías

- [Pyodide](https://pyodide.org/) — CPython compilado a WebAssembly
- [Google Fonts](https://fonts.google.com/) — Orbitron, Share Tech Mono, VT323
- HTML5 Canvas — matrix rain effect
- Vanilla JS — sin frameworks

---

## 📜 Licencia

MIT
