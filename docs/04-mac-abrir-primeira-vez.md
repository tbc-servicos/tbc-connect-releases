# Mac: abrir o app pela primeira vez

No Mac, na **primeira vez** que você abre o TBC Connect, aparece um aviso de segurança da Apple. Isso é normal — o app não é assinado pela Apple (custa uma licença anual que ainda não temos). O app é seguro; basta liberar uma vez.

---

## Passo 1 — Instale na pasta Aplicativos

Ao abrir o `.dmg`, **arraste** o TBC Connect para a pasta **Aplicativos**.

![Arrastar para Aplicativos](img/mac-arrastar.png)

Depois, **ejete** o disco (o `.dmg`) — não rode o app de dentro dele.

## Passo 2 — Abra pela primeira vez com clique-direito

Na pasta **Aplicativos**, **clique com o botão direito** no TBC Connect e escolha **Abrir**.

![Clique direito Abrir](img/mac-abrir.png)

No aviso que aparece, clique em **Abrir** de novo.

> Use **clique-direito → Abrir**. Dois cliques normais não funcionam na primeira vez.

A partir daí, o app abre normalmente sempre.

---

## Se aparecer "está danificado e não pode ser aberto"

O macOS marcou o arquivo como baixado da internet. Abra o **Terminal** (Aplicativos → Utilitários → Terminal) e cole:

```bash
xattr -dr com.apple.quarantine "/Applications/TBC Connect.app"
```

Aperte **Enter** e abra o app de novo.

---

← [Voltar ao início](../README.md)
