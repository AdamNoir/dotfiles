# 🌐 Dotfiles


![Preview](./assets/preview.png)


## 🛠️ Especificaciones del Entorno

* **OS:** Ubuntu
* **Terminal:** Ptyxis / Gnome Terminal
* **Shell:** Zsh
* **Fetch Tool:** [Fastfetch](https://github.com/fastfetch-cli/fastfetch)
* **Tipografía:** FiraCode Nerd Font / Envy Code R


```bash
└── dotfiles/
    ├── assets/
    │   ├── wallpapers/
    │   │   └── wall1
    │   ├── profile-pics/
    │   │   └── pic1
    │   └── ascii-logos/
    │       └── logo1
    └── fastfetch/
        └── config.jsonc
```


---

## 🚀 Guía de Instalación y Configuración

### 1. Instalar Símbolos e Iconos (Nerd Fonts)
Para garantizar que todos los iconos de la terminal, prompts y la configuración de `fastfetch` se muestren correctamente mediante *font fallback*, instalamos el paquete global de símbolos:

```bash
# Crear directorio de fuentes del usuario
mkdir -p ~/.local/share/fonts/nerd-symbols
cd ~/.local/share/fonts/nerd-symbols

# Descargar e instalar Nerd Fonts Symbols
wget [https://github.com/ryanoasis/nerd-fonts/releases/latest/download/NerdFontsSymbolsOnly.zip](https://github.com/ryanoasis/nerd-fonts/releases/latest/download/NerdFontsSymbolsOnly.zip)
unzip NerdFontsSymbolsOnly.zip
rm NerdFontsSymbolsOnly.zip

# Actualizar la caché de fuentes
fc-cache -f -v
