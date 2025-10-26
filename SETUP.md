# 🛠️ Guia de Configuração do Ambiente de Desenvolvimento

Este guia vai te ajudar a configurar todo o ambiente necessário para nossa mentoria, desde a criação da sua conta no GitHub até a configuração do VS Code.

## 📝 1. Criando sua conta no GitHub

1. Acesse [github.com](https://github.com)
2. Clique em "Sign up" (cadastrar-se)
3. Preencha as informações:
   - Seu e-mail
   - Crie uma senha
   - Escolha um nome de usuário (será sua identidade no GitHub)
4. Verifique seu e-mail
5. Personalize seu perfil:
   - Adicione uma foto
   - Complete sua bio
   - Adicione informações profissionais

## 💻 2. Instalando o Git

### Para macOS
1. **Usando Homebrew (Recomendado)**
   ```bash
   # Instalar o Homebrew (se ainda não tiver)
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   
   # Instalar o Git
   brew install git
   ```

2. **Alternativa: Usando o Instalador**
   - Baixe o instalador do Git para macOS em [git-scm.com](https://git-scm.com/download/mac)
   - Execute o pacote .dmg baixado
   - Siga as instruções do instalador

### Para Windows
1. Baixe o instalador do Git para Windows em [git-scm.com](https://git-scm.com/download/windows)
2. Execute o instalador baixado
3. Durante a instalação:
   - Mantenha as opções padrão
   - Na tela "Adjusting your PATH environment", selecione "Git from the command line and also from 3rd-party software"
   - Para "Configuring the line ending conversions", escolha "Checkout Windows-style, commit Unix-style line endings"

### Configuração Inicial do Git
Abra o Terminal (macOS) ou PowerShell/Command Prompt (Windows) e execute:
```bash
# Configure seu nome de usuário
git config --global user.name "Seu Nome"

# Configure seu e-mail (use o mesmo do GitHub)
git config --global user.email "seu.email@exemplo.com"

# Configure o editor padrão para o VS Code
git config --global core.editor "code --wait"

# Para macOS: configurar o gerenciamento de credenciais
git config --global credential.helper osxkeychain

# Para Windows: configurar o gerenciamento de credenciais
git config --global credential.helper wincred
```

## 🎨 3. Instalando o Visual Studio Code

### Para macOS
1. Acesse [code.visualstudio.com](https://code.visualstudio.com/)
2. Baixe a versão para macOS
   - Para Apple Silicon (M1/M2): escolha a versão "Apple Silicon"
   - Para Intel: escolha a versão "Intel Chip"
3. Abra o arquivo .zip baixado
4. Arraste o Visual Studio Code.app para a pasta Applications
5. Adicione o comando 'code' ao PATH:
   - Abra o VS Code
   - Pressione Cmd+Shift+P
   - Digite "shell command"
   - Selecione "Shell Command: Install 'code' command in PATH"

### Para Windows
1. Acesse [code.visualstudio.com](https://code.visualstudio.com/)
2. Baixe a versão para Windows
3. Execute o instalador
4. Durante a instalação:
   - Marque todas as opções em "Select Additional Tasks":
     - ✅ Add "Open with Code" action to Windows Explorer file context menu
     - ✅ Add "Open with Code" action to Windows Explorer directory context menu
     - ✅ Register Code as an editor for supported file types
     - ✅ Add to PATH

## 🔧 4. Extensões Essenciais do VS Code

Instale estas extensões clicando no ícone de extensões (Ctrl+Shift+X) e pesquisando por:

1. **GitHub Copilot**
   - Seu assistente de IA para programação
   - Requer ativação com conta GitHub

2. **Live Server**
   - Para visualizar páginas HTML em tempo real
   - ID: `ritwickdey.LiveServer`

3. **Prettier**
   - Formatador de código
   - ID: `esbenp.prettier-vscode`


## 🔄 5. Configurando o GitHub no VS Code

1. No VS Code, pressione `Ctrl+Shift+P`
2. Digite "Git: Clone"
3. Selecione "Clone from GitHub"
4. Autorize o VS Code a acessar sua conta GitHub
5. Siga as instruções de autenticação

## ⚡ 6. Configurações Recomendadas do VS Code

1. Abra as configurações (Ctrl+,)
2. Adicione estas configurações ao seu `settings.json`:
```json
{
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.bracketPairColorization.enabled": true,
    "editor.guides.bracketPairs": true,
    "editor.minimap.enabled": true,
    "editor.wordWrap": "on",
    "editor.linkedEditing": true,
    "files.autoSave": "afterDelay",
    "git.enableSmartCommit": true,
    "git.autofetch": true
}
```

## 🎯 7. Verificando a Instalação

Para garantir que tudo está funcionando:

1. **Verifique o Git**:
```powershell
git --version
```

2. **Verifique o VS Code**:
- Abra o VS Code
- Abra o terminal integrado (Ctrl+`)
- Digite `code --version`

## 🆘 Problemas Comuns e Soluções

### Git não é reconhecido como comando
- Reinstale o Git marcando a opção "Add to PATH"
- Reinicie o computador

### VS Code não abre pelo terminal
#### No Windows:
- Verifique se o VS Code está no PATH
- Reinstale marcando a opção "Add to PATH"

#### No macOS:
- Execute o comando de instalação do 'code' novamente:
  1. Abra o VS Code
  2. Pressione Cmd+Shift+P
  3. Digite "shell command"
  4. Selecione "Shell Command: Install 'code' command in PATH"

### GitHub não autentica no VS Code
#### No Windows:
- Remova as credenciais antigas do Windows Credential Manager
- Tente o processo de autenticação novamente

#### No macOS:
- Abra o Keychain Access
- Procure por "GitHub"
- Remova as credenciais antigas
- Tente o processo de autenticação novamente

### Homebrew não instala no macOS
- Verifique se tem as Command Line Tools instaladas:
  ```bash
  xcode-select --install
  ```
- Se o erro persistir, execute:
  ```bash
  softwareupdate --all --install --force
  ```

## 📚 Links Úteis

- [Documentação do Git](https://git-scm.com/doc)
- [VS Code Getting Started](https://code.visualstudio.com/docs/getstarted/introvideos)
- [GitHub Guides](https://guides.github.com/)
- [GitHub Copilot Documentação](https://docs.github.com/en/copilot)

## ✅ Próximos Passos

Depois de completar todas as configurações:
1. Clone este repositório de mentoria
2. Crie sua primeira branch
3. Faça seu primeiro commit
4. Abra seu primeiro Pull Request

Se precisar de ajuda em qualquer etapa, estou à disposição! 🚀