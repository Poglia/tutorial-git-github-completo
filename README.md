
# Tutorial Git e GitHub Completo 🚀

Conteúdo do curso da **plataforma B7Web**, destrinchado com carinho por mim! 🎓

---

## 🛠️ Instalação do Git

Escolha o instalador apropriado para o seu sistema operacional:

- **Windows**: [Baixar Git para Windows](https://git-scm.com/downloads/win)
- **Mac**: [Baixar Git para Mac](https://git-scm.com/downloads/mac)
- **Linux**: [Baixar Git para Linux](https://git-scm.com/downloads/linux)

### ✅ Após a Instalação

1. **Reinicie seu computador** ou **Abra um novo terminal** para garantir que as variáveis de ambiente foram configuradas corretamente.  
2. Teste se o Git foi instalado com sucesso com o comando: `git --version`  
   Se tudo estiver funcionando, você verá algo como: `git version 2.42.0`.

---

## 📌 Configuração Inicial

Configure seu nome de usuário e e-mail:  
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```

Essas configurações identificam quem está realizando alterações nos repositórios.  
Você pode conferir as configurações feitas com:  
```bash
git config --list
```

Se precisar editar uma configuração específica:  
```bash
git config --global user.name "Novo Nome"
git config --global user.email "novoemail@exemplo.com"
```

---

## 🌟 Criando e Inicializando um Repositório

### 1. Criar uma pasta no seu sistema operacional:

```bash
mkdir nomeDaPasta && cd nomeDaPasta
```
> - mkdir cria o diretório. 
> - cd entra no diretório.

### 2. Inicializar o repositório Git:
Dentro da pasta criada, inicialize o Git com:
```bash
git init
```

Isso criará um repositório Git para começar a versionar seu projeto.

---

## 📂 Adicionando e Comitando Arquivos

### Adicionar arquivos ao repositório:
 - Agora todo arquivo ou pasta criada dentro do seu repositório será validada pelo git.
 - Crie um arquivo **teste.txt** e siga os demais comandos...

```bash
git add .
```

O comando `git add .` adiciona todos os arquivos e mudanças ao stage.  
Se quiser adicionar um arquivo específico, substitua o `.` pelo nome do arquivo, por exemplo:  
```bash
git add arquivo.txt
```

### Fazer o primeiro commit:
Registre as mudanças no repositório com:
```bash
git commit -m "Primeiro commit"
```

A flag `-m` permite adicionar uma mensagem descritiva ao commit.

---

## 🔗 Conectando ao GitHub

### Criar um repositório no GitHub:
1. Acesse sua conta no [GitHub](https://github.com/).
2. Clique em **New Repository**.
3. Dê um nome ao repositório, configure como público ou privado, e clique em **Create Repository**.

### Conectar o repositório local ao GitHub:
No terminal, use os comandos:  
```bash
git remote add origin https://github.com/seu-usuario/seu-repositorio.git
```

Confirme que o repositório remoto foi adicionado:  
```bash
git remote -v
```

### Enviar arquivos para o GitHub:
Envie seu commit inicial para o repositório remoto:  
```bash
git branch -M main
git push -u origin main
```

---

## 🔄 Fluxo de Trabalho com Git

1. **Verificar status do repositório**:  
   Use `git status` para verificar mudanças ou arquivos não rastreados.

2. **Adicionar mudanças**:  
   Use `git add .` ou `git add nome-do-arquivo`.

3. **Realizar um commit**:  
   Use `git commit -m "Mensagem do commit"`.

4. **Enviar para o repositório remoto**:  
   Use `git push`.

---

Pronto! Agora você sabe como criar, configurar e trabalhar com Git e GitHub. 🚀  
Continue explorando comandos avançados para otimizar seu fluxo de trabalho!
