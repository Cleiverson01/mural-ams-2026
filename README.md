# 🧱 Mural da Turma · AMS 2026

Um mural na internet onde **cada aluno coloca o seu cartão**: nome, um emoji e uma frase sobre o que quer criar com tecnologia.

👉 **Veja o mural no ar:** https://medinagui.github.io/mural-ams-2026/
📄 **Slides e apostila da aula:** [slides.pdf](docs/slides.pdf) · [apostila.pdf](docs/apostila.pdf)

O mais legal é **como** o cartão chega lá. Você vai usar o mesmo caminho que programadores do mundo todo usam para colaborar em projetos de verdade:

1. Você **cria um arquivo** com o seu cartão.
2. Você **pede para juntar** o seu arquivo ao projeto (isso se chama *pull request*).
3. Um **robô** confere se está tudo certo e responde ✅ ou ❌.
4. O instrutor **revisa e aprova** (isso se chama *merge*).
5. O site **se atualiza sozinho** e o seu cartão aparece no mural. 🎉

---

## 📖 Mini dicionário

| Palavra | O que é | Comparando com… |
|---|---|---|
| **Repositório** (repo) | A pasta do projeto, guardada no GitHub, com todo o histórico | Uma pasta compartilhada que lembra de tudo |
| **Commit** | Salvar uma mudança, com uma mensagem dizendo o que mudou | Salvar o jogo (checkpoint) |
| **Fork** | A sua cópia do projeto, na sua conta | "Fazer uma cópia" de um Google Docs de outra pessoa: a cópia é sua, o original continua igual |
| **Pull request** (PR) | Pedido para juntar a sua mudança ao projeto original | Entregar o trabalho pro professor corrigir |
| **Merge** | Juntar de vez a mudança ao projeto | O trabalho corrigido indo para o mural da sala |
| **O robô** (GitHub Actions) | Um programa que roda sozinho a cada PR e confere as regras | O fiscal da prova que confere se você preencheu o nome |
| **GitHub Pages** | Serviço do GitHub que transforma o projeto em site | A vitrine da loja |

---

## ✍️ Como mandar o seu cartão (tudo pelo navegador)

> Você precisa estar **logado** no GitHub. Não tem conta? Crie em https://github.com/signup (é grátis).

**1. Faça a sua cópia do projeto (fork)**
Entre em https://github.com/Medinagui/mural-ams-2026 e clique no botão **Fork**, no canto de cima à direita. Na tela seguinte, clique em **Create fork**.
Pronto: agora você está na **sua cópia**. Repare que no topo aparece o **seu nome de usuário** antes de `mural-ams-2026`. Os próximos passos são todos aqui, na sua cópia.

**2. Entre na pasta de cartões e crie um arquivo novo**
Clique na pasta **`cartoes`**. Lá dentro, clique em **Add file** → **Create new file**.
⚠️ O arquivo **tem** que ficar dentro da pasta `cartoes/`. Se ficar fora, o robô não aceita.

**3. Dê nome ao arquivo**
No campo do nome, escreva o seu **primeiro nome**, em **letras minúsculas**, **sem acento** e terminando em **`.json`**:

```
ana.json        joao.json        maria-clara.json
```

Se já existir alguém com o seu nome, acrescente algo: `joao-2.json` ou `joao-p.json`.

**4. Escreva o seu cartão**
Copie o modelo abaixo, cole na área grande de texto e troque o que está entre aspas:

```json
{
  "nome": "Ana",
  "emoji": "🎮",
  "frase": "Com tecnologia eu quero criar jogos que ensinam matemática",
  "cor": "rosa"
}
```

⚠️ Mantenha as **aspas** `"` e as **vírgulas** no fim das linhas (menos na última linha antes do `}`).

**5. Salve (commit)**
Clique em **Commit changes…**. Na janela que abrir, escreva uma mensagem como `Cartão da Ana`, deixe marcado **Commit directly to the main branch** e clique em **Commit changes**.

**6. Abra o pull request**
Ainda na sua cópia, aparece uma faixa dizendo **"This branch is 1 commit ahead of Medinagui/mural-ams-2026:main"** (a sua cópia tem 1 mudança a mais que o projeto original). Na mesma faixa, clique em **Contribute** → **Open pull request**. Na tela seguinte, clique em **Create pull request**.

**7. Espere o robô 🤖**
Em alguns segundos, o robô comenta no seu pull request:

- ✅ **Tudo certo!** Agora é só esperar o instrutor aprovar.
- 🔧 **Quase lá!** O robô diz exatamente o que arrumar. Para consertar: aba **Files changed** → **três pontinhos (⋯)** do arquivo → **Edit file** → arrume → **Commit changes**. O robô confere de novo sozinho.
- 🔁 **Recomeçar:** se você criou o arquivo fora da pasta `cartoes/` (ou mexeu em outro arquivo), o robô explica passo a passo: fechar o pull request, apagar o arquivo errado na sua cópia e criar de novo no lugar certo.

**8. Olhe para a TV 📺**
Quando o instrutor fizer o merge, em mais ou menos um minuto o seu cartão aparece no mural!

---

## 📏 Regras do cartão

| Campo | O que colocar | Regras |
|---|---|---|
| `nome` | Seu primeiro nome | Só o primeiro nome, **sem sobrenome**. Até 20 letras. Pode ter acento e hífen (`Ana-Clara`). |
| `emoji` | 1 emoji que tenha a sua cara | Exatamente **1** emoji. |
| `frase` | Complete: *"Com tecnologia eu quero criar…"* | Até **80 caracteres**. Sem links, telefone ou e-mail. Sem palavrão. |
| `cor` | A cor do seu cartão | Uma destas: 🟥 `vermelho` · 🟧 `laranja` · 🟨 `amarelo` · 🟩 `verde` · 🩵 `turquesa` · 🟦 `azul` · 🟪 `roxo` · 🩷 `rosa` |

E mais:

- Cada pessoa manda **1 cartão**, só dentro da pasta `cartoes/`.
- Não dá para mexer no cartão dos outros (o robô percebe 😄).

**Como achar um emoji?** No Windows, aperte a tecla **Windows + .** (ponto). No celular, use o teclado de emojis. Ou copie de https://emojipedia.org.

---

## 🔒 Privacidade

Este repositório e o site são **públicos**: qualquer pessoa na internet pode ver. Por isso, só o **primeiro nome**, nada de sobrenome, foto, telefone, e-mail ou endereço. O robô ajuda a conferir, mas a responsabilidade é de todo mundo.

---

## 🔍 Para os curiosos: o que tem aqui dentro?

```
cartoes/            ← os cartões, 1 arquivo por pessoa (é aqui que você mexe!)
site/               ← a página do mural (HTML, CSS e JavaScript)
robo/               ← o "cérebro" do robô, escrito em JavaScript (Node.js)
.github/workflows/  ← as instruções que dizem QUANDO o robô trabalha
```

- **`.github/workflows/robo.yml`**: quando alguém abre um pull request, o GitHub liga um computador na nuvem, roda o robô e mostra ✅ ou ❌. Isso é **CI** (*Integração Contínua*): conferir cada mudança antes de juntar.
- **`.github/workflows/publicar.yml`**: quando o instrutor faz o merge, o GitHub monta o site e coloca no ar. Isso é **CD** (*Entrega Contínua*): publicar sozinho, sem ninguém copiar arquivo na mão.

Quer ver o mural no seu computador? Com o [Node.js](https://nodejs.org) instalado, dentro desta pasta:

```bash
node robo/montar-site.js    # junta os cartões
node robo/servir.js         # abre em http://localhost:8080
node --test robo/regras.test.js   # roda os testes do robô
```

---

Aula ministrada por Guilherme Medina (Thompson Tecnologia) para a turma do AMS · Centro Paula Souza, em 23/10/2026.
