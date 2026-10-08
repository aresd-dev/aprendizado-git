# Boas práticas de Git e GitHub

1. **Faça commits pequenos e com mensagens descritivas.**
   Cada commit deve representar uma mudança lógica única, com uma mensagem que explique o que mudou e por quê (ex.: `docs: adiciona boas práticas de Git`). Isso facilita revisar, reverter e entender o histórico.

2. **Trabalhe em branches, não direto na `main`.**
   Crie uma branch para cada funcionalidade ou correção (ex.: `feature/boas-praticas`) e leve as mudanças para a `main` por Pull Request. Assim a `main` permanece estável e todo código passa por revisão.

3. **Use Pull Requests para revisar antes de mesclar.**
   Descreva o objetivo da mudança, revise o diff com atenção e só faça o merge depois de aprovado. O PR documenta as decisões tomadas e dá espaço para feedback.

4. **Atualize sua `main` local com frequência.**
   Antes de começar algo novo, rode `git checkout main` e `git pull` para evitar conflitos e partir sempre da versão mais recente.

5. **Nunca versione segredos.**
   Senhas, tokens e chaves de API não devem entrar no repositório. Use variáveis de ambiente e um `.gitignore` bem configurado.
