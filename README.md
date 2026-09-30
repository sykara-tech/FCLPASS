# FCL System — Terminal Blindado

Sistema de PDV / cartões para eventos (Firebase Realtime Database).

## Arquivos

| Arquivo | Descrição |
|---------|-----------|
| `login.html` | Tela de autenticação (Balcão + Controladoria) com rodapé SyKaraTech |
| `index.html` | Aplicação principal (PDV, consulta, cartões, gerência, dashboard) |

## Como usar

1. Hospede os dois arquivos na **mesma pasta** (GitHub Pages, Netlify, etc.).
2. Abra `login.html` (ou configure-o como página inicial).
3. Após autenticar, o sistema redireciona para `index.html`.
4. Logout volta para o login.

### Credenciais padrão (Controladoria)

- Usuário: `root`
- Senha: `fcl123`

### Operação Balcão

- Selecione o evento e informe o token/senha cadastrado no Firebase (`eventos`).

## Melhorias nesta versão

- Login separado do app (código mais limpo e carregamento mais leve na autenticação).
- Rodapé SyKaraTech no login alinhado à identidade visual (fundo escuro, logo verde, botão “Acesse nosso site”).
- Sessão persistente via `localStorage` com redirecionamento automático.
- Logout limpa a sessão e retorna ao login.
- Crédito SyKaraTech discreto no rodapé do app.

## Dependências (CDN)

- Firebase App + Database (compat 10.8.0)
- html5-qrcode, Chart.js, QRious, Font Awesome 6, Google Fonts Inter
