
# 🚀 Guia Rápido: Configuração Completa do VSCode para Desenvolvimento

Este guia configura o **Visual Studio Code (VSCode)** do zero para desenvolvimento em **Python, Django, JavaScript, HTML, CSS, C, C++** e outras linguagens populares.

Você terá:

- ✅ Execução de código no terminal
- ✅ Suporte completo a múltiplas linguagens
- ✅ Tema escuro com fonte em itálico (Dracula OM)
- ✅ Ícones de arquivos com estilo Angular Material
- ✅ Terminal e navegação otimizados
- ✅ Aparência visual moderna e agradável

---

## 🧱 1. Instale o VSCode

Baixe o Visual Studio Code em:  
👉 [https://code.visualstudio.com/](https://code.visualstudio.com/)

---

## 🧩 2. Instale extensões essenciais

Abra o VSCode e vá até o **gerenciador de extensões**:

```
Ctrl + Shift + X
```

Instale as extensões abaixo:

| Nome | ID | Função |
|------|----|--------|
| Python | `ms-python.python` | Suporte a Python e Django |
| Code Runner | `formulahendry.code-runner` | Executa código de várias linguagens |
| C/C++ | `ms-vscode.cpptools` | Suporte a C e C++ |
| Prettier | `esbenp.prettier-vscode` | Formatador de código |
| Live Server | `ritwickdey.LiveServer` | Servidor para projetos Web |
| Django | `batisteo.vscode-django` | Snippets e suporte para Django |
| Material Icon Theme | `PKief.material-icon-theme` | Ícones modernos de arquivos |
| OM Theme | `LuisOtavioDev.om-theme` | Tema escuro baseado no Dracula |

Você também pode instalar todas com este comando:

```bash
code --install-extension ms-python.python      --install-extension formulahendry.code-runner      --install-extension ms-vscode.cpptools      --install-extension esbenp.prettier-vscode      --install-extension ritwickdey.LiveServer      --install-extension batisteo.vscode-django      --install-extension PKief.material-icon-theme      --install-extension LuisOtavioDev.om-theme
```

---

## 🎨 3. Ativar tema e ícones

Abra a paleta de comandos:

```
Ctrl + Shift + P
```

E execute os seguintes comandos:

- `Preferences: Color Theme` → selecione **OM Theme (Default Dracula Italic)**
- `Preferences: File Icon Theme` → selecione **Material Icon Theme**

---

## ⚙️ 4. Substituir configurações do VSCode

Abra o arquivo `settings.json`:

```
Ctrl + Shift + P → Preferences: Open User Settings (JSON)
```

Apague o conteúdo existente e cole o seguinte:

---

## 📄 settings.json completo

```json
{
    "explorer.compactFolders": false,
    "code-runner.runInTerminal": true,
    "workbench.startupEditor": "none",
    "code-runner.clearPreviousOutput": true,
    "code-runner.executorMap": {
        "javascript": "node",
        "java": "cd $dir && javac $fileName && java $fileNameWithoutExt",
        "c": "cd $dir && gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "zig": "zig run",
        "cpp": "cd $dir && g++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "objective-c": "cd $dir && gcc -framework Cocoa $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "php": "php",
        "python": "cls ; python -u",
        "perl": "perl",
        "perl6": "perl6",
        "ruby": "ruby",
        "go": "go run",
        "lua": "lua",
        "groovy": "groovy",
        "powershell": "powershell -ExecutionPolicy ByPass -File",
        "bat": "cmd /c",
        "shellscript": "bash",
        "fsharp": "fsi",
        "csharp": "scriptcs",
        "vbscript": "cscript //Nologo",
        "typescript": "ts-node",
        "coffeescript": "coffee",
        "scala": "scala",
        "swift": "swift",
        "julia": "julia",
        "crystal": "crystal",
        "ocaml": "ocaml",
        "r": "Rscript",
        "applescript": "osascript",
        "clojure": "lein exec",
        "haxe": "haxe --cwd $dirWithoutTrailingSlash --run $fileNameWithoutExt",
        "rust": "cd $dir && rustc $fileName && $dir$fileNameWithoutExt",
        "racket": "racket",
        "scheme": "csi -script",
        "ahk": "autohotkey",
        "autoit": "autoit3",
        "dart": "dart",
        "pascal": "cd $dir && fpc $fileName && $dir$fileNameWithoutExt",
        "d": "cd $dir && dmd $fileName && $dir$fileNameWithoutExt",
        "haskell": "runghc",
        "nim": "nim compile --verbosity:0 --hints:off --run",
        "lisp": "sbcl --script",
        "kit": "kitc --run",
        "v": "v run",
        "sass": "sass --style expanded",
        "scss": "scss --style expanded",
        "less": "cd $dir && lessc $fileName $fileNameWithoutExt.css",
        "FortranFreeForm": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "fortran-modern": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "fortran_fixed-form": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "fortran": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "sml": "cd $dir && sml $fileName",
        "mojo": "mojo run",
        "erlang": "escript",
        "spwn": "spwn build",
        "pkl": "cd $dir && pkl eval -f yaml $fileName -o $fileNameWithoutExt.yaml",
        "gleam": "gleam run -m $fileNameWithoutExt"
    },
    "code-runner.ignoreSelection": true,
    "workbench.colorTheme": "OM Theme (Default Dracula Italic)",
    "workbench.iconTheme": "material-icon-theme",
    "python.defaultInterpreterPath": "python",
    "cSpell.language": "pt, en",
    "cSpell.enabled": false
}
```

---

## ✅ Tudo pronto!

Seu VSCode agora está totalmente preparado para:

- Python e Django 🐍  
- Web com HTML, CSS, JS e Live Server 🌐  
- C, C++, Rust, Go, Java e outras linguagens ⚙️  
- Aparência estilizada e terminal funcional 💻  

---

Boas codificações! 🚀


---

## 🖥️ Instruções Específicas por Sistema Operacional

### 🪟 Windows

- **Python**: Baixe e instale em [https://www.python.org/](https://www.python.org/). Marque a opção **"Add Python to PATH"** durante a instalação.
- **GCC (C/C++)**: Instale via [MSYS2](https://www.msys2.org/) ou o [MinGW-w64](http://mingw-w64.org/).
- **Node.js**: Instale em [https://nodejs.org/](https://nodejs.org/)
- **Java**: Instale o JDK em [https://adoptium.net/](https://adoptium.net/)
- **Extensões**: Use `Ctrl + Shift + X` ou instale pela CLI com `code --install-extension`.

### 🍎 macOS

- **Python, Node.js, Git, GCC**: Instale o Homebrew:  
  ```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```
  Em seguida:
  ```bash
  brew install python node git gcc
  ```
- **Java**:  
  ```bash
  brew install openjdk
  ```
- **Xcode Tools (compiladores C/C++)**:  
  ```bash
  xcode-select --install
  ```

### 🐧 Linux (Ubuntu/Debian)

Atualize o sistema:
```bash
sudo apt update && sudo apt upgrade -y
```

Instale as ferramentas principais:
```bash
sudo apt install build-essential python3 python3-pip nodejs npm git default-jdk -y
```

Instale o VSCode:
```bash
sudo snap install code --classic
```

---

Pronto! Com tudo isso, seu VSCode estará funcionando perfeitamente em qualquer sistema.
