<div align="center">

# ⚡ NvimConfig

**Мой конфиг Neovim — клонируй и работай на любой системе**

[![Neovim](https://img.shields.io/badge/Neovim-57A143?style=flat-square&logo=neovim&logoColor=white)](https://neovim.io/)
[![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua&logoColor=white)](https://www.lua.org/)
[![Gentoo](https://img.shields.io/badge/Gentoo-54487A?style=flat-square&logo=gentoo&logoColor=white)](https://www.gentoo.org/)
[![Debian](https://img.shields.io/badge/Debian-A81D33?style=flat-square&logo=debian&logoColor=white)](https://www.debian.org/)
[![Arch](https://img.shields.io/badge/Arch-1793D1?style=flat-square&logo=archlinux&logoColor=white)](https://archlinux.org/)
[![macOS](https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white)](https://www.apple.com/macos/)

[📥 Установка](#-установка) • [🔄 Обновление](#-обновление) • [🗑️ Удаление](#-удаление)

</div>

---

## 📋 Содержание

- [🚀 Установка](#-установка)
- [🔄 Обновление](#-обновление)
- [🗑️ Удаление](#-удаление)

---

## 🚀 Установка

### 1️⃣ Удалить старое

```bash
rm -rf ~/.config/nvim ~/.local/share/nvim ~/.local/state/nvim ~/.cache/nvim
```

> [!CAUTION]
> ⚠️ **Внимание!** Эта команда полностью удаляет текущий конфиг, плагины и кэш.
>
> Если есть что-то ценное — сначала сделай бэкап:
>
> ```bash
> cp -r ~/.config/nvim ~/nvim-backup
> ```

### 2️⃣ Установить зависимости

<details>
<summary><b>🐧 Gentoo</b></summary>

```bash
sudo emerge --ask dev-vcs/git net-libs/nodejs app-editors/neovim
```

</details>

<details>
<summary><b>🐧 Debian / Ubuntu</b></summary>

```bash
sudo apt install git npm neovim
```

</details>

<details>
<summary><b>🐧 Arch Linux</b></summary>

```bash
sudo pacman -S git npm neovim
```

</details>

<details>
<summary><b>🍎 macOS</b></summary>

```bash
brew install git npm neovim
```

</details>

#### 📦 Зачем нужны эти пакеты?

| Пакет | Назначение |
|:------|:-----------|
| `neovim` | 📝 Сам редактор |
| `git` | 📥 Скачать этот конфиг |
| `npm` | 🔌 LSP-серверы и провайдеры |

### 3️⃣ Склонировать конфиг

```bash
git clone https://github.com/RayAIl/NvimConfig.git ~/.config/nvim
```

### 4️⃣ Запустить Neovim

```bash
nvim
```

> [!TIP]
> 💡 При первом запуске плагины установятся автоматически.
>
> После установки запусти `:checkhealth` и убедись, что все зависимости на месте.

---

## 🔄 Обновление

Обновить конфиг до последней версии очень просто:

```bash
cd ~/.config/nvim && git pull
```

Просто перезапусти `nvim` — и всё готово! ✨

---

## 🗑️ Удаление

Чтобы полностью удалить конфиг и все связанные данные:

```bash
rm -rf ~/.config/nvim ~/.local/share/nvim ~/.local/state/nvim ~/.cache/nvim
```

> [!NOTE]
> 📝 После удаления конфигурация вернётся к стандартному виду Neovim.

---

<div align="center">

**Сделано с ❤️и ☕**

[![GitHub](https://img.shields.io/badge/GitHub-RayAIl-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/RayAIl)

</div>
