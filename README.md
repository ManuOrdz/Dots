# Configuración de Neovim (nvim)

¡Bienvenido al repositorio de configuración personalizada de Neovim! Este proyecto tiene como objetivo proporcionar una configuración optimizada, modular y fácil de mantener para desarrolladores que utilizan Neovim como editor principal. A continuación, encontrarás instrucciones para la instalación, organización de los archivos, plugins utilizados y cómo extender la configuración según tus necesidades.

---

## Contenido

- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Estructura del repositorio](#estructura-del-repositorio)
- [Plugins principales](#plugins-principales)
- [Atajos de teclado](#atajos-de-teclado)
- [Soporte para lenguajes](#soporte-para-lenguajes)
- [Temas y personalización](#temas-y-personalización)
- [Cómo contribuir](#cómo-contribuir)

---

## Requisitos

- **Neovim** v0.9 o superior  
- **Git** para la instalación de plugins  
- **Python** con soporte para `pynvim`:  

  ```bash
  pip install pynvim
  ```

- **Ripgrep** (opcional pero recomendado para búsquedas rápidas)

---

## Instalació> [!NOTE]

``` $ bash
git clone https://github.com/ManuOrdz/Nvim-Dots.git ~/.config/nvim
```

---

## Plugins principales

Esta configuración incluye algunos de los plugins más populares para mejorar la productividad:

- **[Telescope](https://github.com/nvim-telescope/telescope.nvim)**: Búsqueda y navegación rápida.
- **[Treesitter](https://github.com/nvim-treesitter/nvim-treesitter)**: Resaltado de sintaxis avanzado.
- **[Lualine](https://github.com/nvim-lualine/lualine.nvim)**: Barra de estado personalizable.

## Atajos de teclado

Algunos de los atajos de teclado más útiles definidos en esta configuración son:

- **`<leader>ff`**: Buscar archivos con Telescope.
- **`<leader>fg`**: Buscar texto dentro del proyecto.
- **`<leader>q`**: Cerrar ventana actual.
- **`<leader>w`**: Guardar cambios.
- **`gd`**: Ir a la definición de una función/clase (LSP).
- **K**: Mostrar documentación flotante.

Puedes personalizar estos atajos editando el archivo `lua/keymaps.lua`.

---

## Soporte para lenguajes

Esta configuración proporciona soporte para varios lenguajes a través del cliente LSP y plugins adicionales:

- **Python**: Configurado con `pyright`.
- **Lua**: Optimización para la configuración de Neovim.
  
## Temas y personalización

El tema por defecto de esta configuración es **kanagawa**. Sin embargo, puedes cambiarlo fácilmente:

1. Abre el archivo `lua/settings.lua`.
2. Cambia el nombre del tema en la sección correspondiente:

   ```lua
   vim.cmd("colorscheme kanagawa")
   ```
