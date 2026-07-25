# Mac: abrir o app pela primeira vez

No Mac, na **primeira vez** que você abre o TBC Connect, aparece um aviso de segurança da Apple. Isso é normal — o app não é notarizado pela Apple (custa uma licença anual que ainda não temos). O app é seguro; basta liberar uma vez.

O aviso costuma dizer:

> "A Apple não pôde verificar se o item TBC Connect está livre de algum malware capaz de danificar o Mac ou comprometer sua privacidade."

---

## Passo 1 — Instale na pasta Aplicativos

Ao abrir o `.dmg`, **arraste** o TBC Connect para a pasta **Aplicativos**.

![Arrastar para Aplicativos](img/mac-arrastar.png)

Depois, **ejete** o disco (o `.dmg`) — não rode o app de dentro dele.

## Passo 2 — Libere o app

O caminho **mudou no macOS Sequoia (15)**. Veja qual é a sua versão em  → Ajustes do Sistema → Geral → Sobre.

### macOS 15 (Sequoia) ou mais novo

O clique-direito → Abrir **não funciona mais** nessas versões — a Apple removeu esse atalho. Faça assim:

1. Tente abrir o app normalmente (dois cliques). O aviso aparece — clique em **OK**.
2. Abra **Ajustes do Sistema → Privacidade e Segurança**.
3. Role até o fim. Vai haver uma linha dizendo que o *TBC Connect* foi bloqueado.
4. Clique em **Abrir Assim Mesmo** e confirme com Touch ID ou senha.

A partir daí o app abre normalmente sempre.

### macOS 14 (Sonoma) ou mais antigo

Na pasta **Aplicativos**, **clique com o botão direito** no TBC Connect e escolha **Abrir**.

![Clique direito Abrir](img/mac-abrir.png)

No aviso que aparece, clique em **Abrir** de novo.

> Use **clique-direito → Abrir**. Dois cliques normais não funcionam na primeira vez.

---

## Passo 3 — Permissões de gravação (só se for usar as Gravações)

Para gravar reuniões o macOS exige duas permissões. Elas **não** são pedidas na instalação, só na primeira gravação.

Em **Ajustes do Sistema → Privacidade e Segurança**:

- **Microfone** → ligue o TBC Connect
- **Gravação de Tela** → ligue o TBC Connect

> A permissão de **Gravação de Tela** é o que libera o **áudio do sistema** — a voz das outras pessoas na call. O app não grava imagem nenhuma: a faixa de vídeo é descartada assim que chega. É assim que a Apple expõe esse áudio, não há outro caminho.

Se essa permissão faltar, o app avisa na tela que gravou **só o microfone**, em vez de gravar silêncio sem você perceber.

⚠️ **A cada atualização do app essas permissões precisam ser concedidas de novo.** Como o app é assinado ad-hoc, o identificador muda a cada versão e o macOS trata como se fosse outro app. Some quando tivermos a licença de desenvolvedor da Apple.

---

## Alternativa pelo Terminal

Se preferir resolver de uma vez, sem passar pelos Ajustes:

```bash
xattr -dr com.apple.quarantine "/Applications/TBC Connect.app"
```

Isso remove a marca de "baixado da internet" e o app abre direto. Use só em app que você sabe de onde veio — é o nosso caso.

## Se aparecer "está danificado e não pode ser aberto"

Mensagem diferente da anterior, e mais grave: indica assinatura inválida, não apenas falta de notarização. Aconteceu na v0.7.0 e foi corrigido na v0.7.1. Rode o comando do Terminal acima; se persistir, avise — aí é bug de empacotamento, não configuração da sua máquina.

---

← [Voltar ao início](../README.md)
