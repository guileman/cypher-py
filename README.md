# CYPHER.PY — Learn Python or Die Trying

> Un juego de aprendizaje de Python con estética hacker/ciberpunk. Python real en el navegador via Pyodide. Sin servidor. Listo para GitHub Pages.

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
- **12 misiones** progresivas: básico → intermedio → avanzado
- **Sistema de XP y niveles**
- Estética ciberpunk: matrix rain, scanlines, CRT glow
- Un solo archivo `index.html` — cero dependencias locales
- **Tab** para indentar, **Ctrl+Enter** para ejecutar código

---

## 📋 Misiones

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

---

## 🔧 Cómo agregar misiones

En `index.html`, dentro del array `missions`:

```javascript
{
  id: 'M-013',
  name: 'Nombre',
  diff: 'basico' | 'intermedio' | 'avanzado',
  xp: 50,
  story: 'Narrativa...',
  objective: 'Qué debe hacer el jugador (HTML permitido)',
  hint: 'Pista en texto plano',
  starter: '# código inicial\n\n',
  validate: (output) => output.trim() === 'resultado esperado'
}
```

---

## 📁 Estructura

```
cypher-py/
├── index.html   ← todo el juego
└── README.md
```

## 📜 Licencia

MIT
