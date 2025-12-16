# DevCards - Minicurso Git/GitHub

## Slides do minicurso
[Minicurso Git/GitHub](https://www.canva.com/design/DAGkSRP0LUI/ouSMNMFtEqKbuL_llIP_4w/edit?utm_content=DAGkSRP0LUI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Notion Git/Git Hub:
[Notion](https://www.notion.so/Git-na-pr-tica-1c2acd2f0b358081a321ec87fc40edd1?source=copy_link)

## Objetivo do Projeto

Criar uma página web colaborativa onde cada participante do minicurso adicionará seu próprio **card de perfil tech**, praticando o fluxo completo de trabalho com Git e GitHub em um cenário real de desenvolvimento colaborativo.

O objetivo principal é consolidar os conhecimentos do curso através da **execução prática** de um fluxo de trabalho padrão da indústria, desde a criação de uma branch até a abertura de um Pull Request.

---

## Descrição do Projeto

**DevCards da Turma** é uma aplicação web que exibe cards com informações técnicas de cada aluno. Cada card contém:

- Nome completo
- Área tech de interesse/preferência
- Linguagem de programação favorita
- Meta profissional na tecnologia
- Descrição de um projeto dos sonhos
- Uma tag/palavra que representa o aluno

## Layout Base

O projeto já possui:
- Estrutura HTML inicial
- Estilos CSS modernos (gradientes, efeitos visuais, responsividade)
- Card modelo para orientação
- Design pronto para receber novas contribuições

---

## Fluxo de Trabalho - PASSO A PASSO

### **ETAPA 1: Configuração Inicial**

1. **Clonar o Repositório**
```bash
# Clone o repositório para sua máquina local
git clone https://github.com/seu-usuario/DevCards.git

# Entre na pasta do projeto
cd DevCards
```

### **ETAPA 2: Escolha e Atribuição da Tarefa**

1. **Acessar as Issues**
   - Vá até a aba "Issues" do repositório
   - Localize a issue com seu nome: `Adicionar card: [SEU NOME]`

2. **Revisar os Critérios de Aceite**
   - Leia cuidadosamente todos os requisitos da issue
   - Certifique-se de entender o que precisa ser feito

3. **Atribuir a Issue a Você** (se necessário)
   - Na issue, clique em "Assign yourself"

### **ETAPA 3: Trabalhando na Sua Branch**

1. **Atualizar a Branch dev Local**
```bash
# Certifique-se de estar na branch dev
git checkout dev

# Baixe as últimas alterações
git pull origin dev

```

2. **Criar Sua Branch de Trabalho**
```bash
# Crie uma nova branch a partir de dev
# Use o padrão: feat/add-card-seunome
git checkout -b feat/add-card-seunome dev
```

3. **Desenvolver sua Funcionalidade**
   - Abra o arquivo `index.html` em seu editor
   - Localize o comentário: `<!-- OS NOVOS CARDS DOS ALUNOS SERÃO ADICIONADOS AQUI -->`
   - **IMPORTANTE:** Adicione seu card **ACIMA** deste comentário
   - **NÃO** modifique cards de outros alunos
   - **NÃO** apague o card modelo

4. **Formato do Seu Card**
```html
<div class="card">
  <div class="card-header">
    <i class="fas fa-user"></i>
    <h2>SEU NOME COMPLETO</h2>
  </div>
  <div class="info"><i class="fas fa-laptop-code"></i> Área Favorita: [ex: Frontend, Backend, Dados]</div>
  <div class="info"><i class="fas fa-code"></i> Linguagem: [ex: Python, JavaScript, Java]</div>
  <div class="info"><i class="fas fa-bullseye"></i> Meta: [ex: Desenvolvedor Full-Stack]</div>
  <div class="info"><i class="fas fa-star"></i> Projeto dos Sonhos: [descrição breve]</div>
  <div class="tag"><i class="fas fa-tag"></i> [uma palavra que te descreva]</div>
</div>
```

### **ETAPA 4: Commit e Push**

1. **Verificar suas Alterações**
```bash
# Veja quais arquivos foram modificados
git status
```

2. **Adicionar e Commitar**
```bash
# Adicione o arquivo modificado
git add index.html

# Faça um commit com mensagem semântica
git commit -m "feat: adiciona card de [Seu Nome]"
```

3. **Enviar para o GitHub**
```bash
# Faça o push da sua branch
git push origin feat/add-card-seunome
```

### **ETAPA 5: Criar Pull Request (PR)**

1. **Acessar o Repositório no GitHub**
   - Vá até a página do seu repositório
   - Deverá aparecer um botão "Compare & pull request"

2. **Criar o Pull Request**
   - Clique em "New Pull Request"
   - Selecione:
     - Base: `dev` (do repositório principal)
     - Compare: `feat/add-card-seunome` (sua branch)
   
3. **Preencher Informações do PR**
   - **Título:** `feat: adiciona card de [Seu Nome]`
   - **Descrição:**
     - Referencie a issue: `Resolves #NÚMERO_DA_ISSUE`
     - Descreva brevemente o que foi feito
     - Liste os itens implementados

4. **Revisar e Submeter**
   - Verifique se o diff mostra apenas seu card
   - Clique em "Create Pull Request"

### **ETAPA 6: Aguardar Revisão e Merge**

1. **Responder a Feedback** (se houver)
   - O mantenedor pode solicitar ajustes
   - Faça as correções na mesma branch
   - Faça commit e push novamente

2. **Acompanhar o Status**
   - Verifique se o PR foi aprovado
   - Confirme quando for mesclado (merged)

3. **Atualizar seu Repositório Local**
```bash
# Volte para a branch dev
git checkout dev

# Baixe as alterações mescladas
git pull origin dev
```
