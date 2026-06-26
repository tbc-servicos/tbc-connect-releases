# Como acessar no meu Computador um serviço que está rodando na VM

**Exemplo:** você subiu um sistema na VM (uma aplicação web, um banco, uma API) e quer abrir ele no navegador ou numa ferramenta **do seu computador**.

> Direção usada: **-L Receber**. O serviço sai da VM e chega no seu PC.

---

## Passo 1 — Abra Projetos e crie um novo

Na tela **Projetos**, clique em **+ Novo projeto**.

![Novo projeto](img/projetos-novo.png)

## Passo 2 — Dê um nome

Ex: `App da VM`.

![Nome do projeto](img/projetos-nome.png)

## Passo 3 — Escolha a direção "-L Receber (VM)"

No campo **Direção**, selecione **-L Receber (VM)**.

![Direção -L](img/uso-l-direcao.png)

## Passo 4 — Preencha os campos

| Campo | O que colocar | Exemplo |
|-------|---------------|---------|
| **Serviço na VM** | Já vem como `localhost` — pode deixar | `localhost` |
| **Porta na VM (origem)** | A porta onde o serviço roda **na VM** | `3000` |
| **Porta local (no seu PC)** | Já copia a mesma porta — pode deixar | `3000` |

![Campos preenchidos -L](img/uso-l-campos.png)

Clique em **+ Adicionar redirecionamento** e depois em **Salvar**.

## Passo 5 — Conecte

No card do projeto, clique em **Conectar**.

![Conectar -L](img/uso-l-conectar.png)

## Pronto!

Agora abra no seu computador:

```
http://localhost:3000
```

É o serviço que está rodando na VM, acessível direto do seu PC.

---

← [Voltar ao início](../README.md)
