# TBC Connect

App para acessar os serviços do cliente (Protheus, Git, etc.) direto da VM de desenvolvimento, usando a VPN que está na **sua máquina**.

## 1. Baixe

Escolha o instalador do seu sistema:

| Sistema | Download |
|---------|----------|
| 🪟 **Windows** | [Baixar .exe](https://github.com/tbc-servicos/tbc-connect-releases/releases/latest) |
| 🍎 **Mac** (Apple Silicon / M1, M2…) | [Baixar .dmg](https://github.com/tbc-servicos/tbc-connect-releases/releases/latest) |
| 🍎 **Mac** (Intel) | [Baixar .dmg](https://github.com/tbc-servicos/tbc-connect-releases/releases/latest) |
| 🐧 **Linux** | [Baixar .AppImage](https://github.com/tbc-servicos/tbc-connect-releases/releases/latest) |

Instale e abra. O app se atualiza sozinho — você não precisa voltar aqui.

> 🍎 **No Mac**, na primeira vez aparece um aviso de segurança. Veja [como abrir no Mac](docs/04-mac-abrir-primeira-vez.md).

## 2. Configure (uma vez)

1. Escolha sua **VM** e seu **usuário**.
2. Digite a **senha da VM**. Pronto — o acesso fica salvo.

## 3. Use

1. Crie um **Projeto** e informe as portas que você precisa.
2. Ligue a **VPN do cliente** no seu computador.
3. Clique em **Conectar**.

Agora é só usar `localhost:<porta>` na VM para chegar no serviço do cliente.

---

## 📖 Guias passo a passo (com imagens)

Clique no seu caso para ver como configurar:

- **[Como configurar meu acesso](docs/01-configurar-acesso.md)**
  Primeiro uso: escolher VM, usuário e senha.

- **[Acessar no meu Computador um serviço que roda na VM](docs/02-servico-da-vm-no-computador.md)**
  Ex: abrir no seu navegador um sistema que está rodando na VM.

- **[Acessar na VM um serviço externo (VPN do Cliente)](docs/03-servico-externo-na-vm.md)**
  Ex: fazer a VM chegar no Protheus do cliente usando a VPN que está no seu PC.

- **[Mac: abrir o app pela primeira vez](docs/04-mac-abrir-primeira-vez.md)**
  Como liberar o aviso de segurança da Apple no primeiro uso.

---

Problemas? Fale com o time de infra da TBC.
