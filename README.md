````markdown
<div align="center">

# ⚡ NvimConfig

Мой конфиг Neovim — клонируй и работай на любой системе.

![Neovim](https://img.shields.io/badge/Neovim-57A143?style=flat-square&logo=neovim&logoColor=white)
![Gentoo](https://img.shields.io/badge/Gentoo-54487A?style=flat-square&logo=gentoo&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=flat-square&logo=debian&logoColor=white)
![Arch](https://img.shields.io/badge/Arch-1793D1?style=flat-square&logo=archlinux&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white)

</div>

---

## 🚀 Установка

### 1. Удалить старое

```bash
rm -rf ~/.config/nvim ~/.local/share/nvim ~/.local/state/nvim ~/.cache/nvim
```

> ⚠️ Команда сносит текущий конфиг, плагины и кэш. Если внутри есть что-то ценное —
> сначала сделай бэкап: `cp -r ~/.config/nvim ~/nvim-backup`

### 2. Поставить зависимости

**Gentoo:**

```bash
sudo emerge --ask dev-vcs/git net-libs/nodejs app-editors/neovim
```

**Debian / Ubuntu:**

```bash
sudo apt install git npm neovim
```

**Arch:**

```bash
sudo pacman -S git npm neovim
```

**macOS:**

```bash
brew install git npm neovim
```

| Пакет | Зачем нужен |
|-------|-------------|
| `neovim` | сам редактор |
| `git` | скачать этот конфиг |
| `npm` | LSP-серверы |

### 3. Склонировать конфиг

```bash
git clone https://github.com/RayAIl/NvimConfig.git ~/.config/nvim
```

### 4. Запустить

```bash
nvim
```

При первом запуске плагины установятся автоматически. После — прогони
`:checkhealth` и убедись, что все зависимости на месте.

---

## 🔄 Обновление

```bash
cd ~/.config/nvim && git pull
```

Перезапусти nvim — и всё.

---

## 🗑️ Удаление

```bash
rm -rf ~/.config/nvim ~/.local/share/nvim ~/.local/state/nvim ~/.cache/nvim
```

<!-- сюда можно вставить скриншот:
![preview](screenshots/main.png)
-->
````

Применить у себя:

```bash
cd ~/.config/nvim
nano README.md   # вставить новое содержимое, Ctrl+O, Ctrl+X
git add README.md && git commit -m "README: оформление" && git push
```
````markdown
