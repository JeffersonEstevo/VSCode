

##  *-----------{ CONFIGURAÇÕES VSCODE }----------*

<!-- Comentário segue padrão do HTML-->

<details><summary><b>Python</b></summary>

**COFIGURAÇÕES VSCODE PARA PYTHON**  

+ Para visualizar em tempo real as modificações de Markdown no VSCode utilizamos os atalhos `ctrl`+`k` e `v`.

+ As configurações aqui apresentadas servem para todos os sistemas operacionais

+ Configurações em arquivo no VSCode aparecem quando cilcamos no ícone. ![Settings](imagens/settings.png)
 O arquivo é o `settings.json`

 + O arquivo `settings.json` utilizado estará na raiz deste repositório.

 + Para prepara o interpretador do Python pra executar em possíveis versões de ambientes virtuais que possam estar sendo utilizadas posteriormente, devemos habilitar a opção `python.defaultInterpreterPath` para `true`, para usar a versão do interpretador do Python como padrão.
---

+ Por padrão o VSCode utiliza `compact folders` que exibe a estrutura de pastas com seu caminho completo. Para desativar essa opção clicamos em `configurações -> settings` e procuramos por compact foldes e então desabilitamos.
---

#### Atalhos
> Copy Line Down `Shift`+`Alt`+`DownArrow`  
> Copy Line Up `Shift`+`Alt`+`UpArrow`
---

#### Extensões
> Extensão para Python `Python`  
> Extensão para executar diversas linguagens `Code Runner`

+ Para executar a xtensão no terminal e não na output do VSCode, devemos setar a opção `code-runner.runInTerminal` para `true`, por padrão ela vem setada como false.  

+ Para limpar o terminal após executar qualquer comando devemos setar a opção `code-runner.clearPreviousOutput` para `true`, por padrão ela vem setada como false.
    - Por veze, apenas setar o comando `code-runner.clearPreviousOutput` para true não resolve completamente o problema com alimpeza do terminal, então devemos configurar os comandos a serem utilizados na configuração `code-runner.executorMap` e setar na chave `python` os comandos `cls && python -u` (para o caso do CMD do Windows), `cls ; python -u` (para o caso do PowerShell do Windows) ou `clear && python -u` (para o caso do Linux).  

+ Por padrão, o Code Runner executa apenas parte selecionada no arquivo fonte do VSCdode, para desabilitar essa opção setamos a propriedade `codecode-runner.ignoreSelection` para `true`, por padrão essa opção vem setada como false; 

---

#### Tema

+ Para utilizar o tema desenvolvido por Otávio Miranda (tema baseado no Dracula), devemos ir em extensões e procurar por `omthemes` e instalar o tema `Om Theme (A Darker Dracula Theme)`, em seguida ser perguntado como utilizar o itálico, recomenda-se utilizar a opção padrão para o itálico `OM Theme (Default Dracula Italic)`.

+ Para uma boa exibição da estruturas de pastas no VSCode podemos utilizar o tema padrão do Agular Material, pesquisando por `material icon theme` nas extenões e instalando-a. Após a instalação será exibido o tema que está sendo usado no momento (Seti Visual Studio Code), devemos selecionar o `Material Icon Theme` para modificar.
---

</details>

<details><summary><b>JavaScript</b></summary>

</details>




