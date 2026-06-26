# Como acessar na VM um serviço externo (VPN do Cliente) usando minha VM

**Exemplo:** o cliente tem um servidor (Protheus, Git, banco) que só é alcançável pela **VPN dele**. A VPN está no **seu computador**, mas você precisa que a **VM** chegue nesse servidor.

> Direção usada: **-R Enviar**. Seu PC empresta o acesso da VPN para a VM.

---

## Antes de começar

Ligue a **VPN do cliente** no seu computador. Sem ela, não há o que redirecionar.

---

## Passo 1 — Abra Projetos e crie um novo

Na tela **Projetos**, clique em **+ Novo projeto**.

![Novo projeto](img/projetos-novo.png)

## Passo 2 — Dê um nome

Use o nome do cliente. Ex: `Cassi`.

![Nome do projeto](img/projetos-nome.png)

## Passo 3 — Escolha a direção "-R Enviar (VPN)"

No campo **Direção**, selecione **-R Enviar (VPN)** (é o padrão).

![Direção -R](img/uso-r-direcao.png)

## Passo 4 — Preencha os campos

| Campo | O que colocar | Exemplo |
|-------|---------------|---------|
| **IP do servidor (na VPN)** | O endereço do servidor do cliente | `tfs.cassi.com.br` |
| **Porta no servidor** | A porta do serviço do cliente | `443` |
| **Porta na VM** | A porta onde isso vai aparecer **na VM** | `8443` |

![Campos preenchidos -R](img/uso-r-campos.png)

Clique em **+ Adicionar redirecionamento** e depois em **Salvar**.

## Passo 5 — Conecte

No card do projeto, clique em **Conectar**.

![Conectar -R](img/uso-r-conectar.png)

## Pronto!

Dentro da **VM**, o serviço do cliente agora responde em:

```
localhost:8443
```

A VM usa a sua VPN sem precisar instalar nada nela.

---

← [Voltar ao início](../README.md)
