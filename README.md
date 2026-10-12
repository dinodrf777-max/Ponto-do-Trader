# Ponto do Trader

Jogo educativo de investimentos em uma página HTML.

## Firebase

O jogo usa Firebase Authentication com e-mail/senha e Cloud Firestore para salvar o progresso de cada conta na nuvem.

1. No Firebase Console, ative o provedor **E-mail/senha**.
2. Crie o banco Firestore na região adequada aos jogadores.
3. Publique as regras de `firestore.rules` na guia **Firestore → Regras**.
4. Em **Authentication → Configurações → Domínios autorizados**, inclua `dinodrf777-max.github.io`.
5. Publique `index.html` com GitHub Pages.

Os saldos do jogo são fictícios. Cada jogador pode gravar somente seu próprio progresso. Para habilitar o painel administrativo, crie primeiro a conta do administrador no app e, em seguida, crie no Firestore um documento vazio em `admins/{UID}`, usando o UID dessa conta exibido em **Authentication → Usuários**. Não permita que o app crie documentos nessa coleção.

## GitHub Pages

Em **Settings → Pages**, selecione **Deploy from a branch**, escolha `main` e `/ (root)`.
