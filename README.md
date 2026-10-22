# Fitmais — Controle de alunos por professor (protótipo)

Protótipo navegável do sistema de distribuição de alunos por professor, feito pela Evolue Treinamento e Desenvolvimento para demonstração comercial.

**Os dados são fictícios.** Nenhum aluno, professor ou treino aqui é real, e nada é enviado para servidor: tudo fica salvo apenas no navegador de quem abre a página.

## Publicar no GitHub Pages

1. Crie um repositório (sugestão de nome: `fitmais-demo`).
2. Envie os arquivos `index.html`, `README.md` e `.nojekyll` para a branch principal.
3. Em **Settings → Pages**, escolha a branch principal e a pasta raiz (`/root`).
4. Em poucos minutos o link fica no ar, no formato `https://<usuario>.github.io/fitmais-demo/`.

## O que mostrar na demonstração

- **Operação:** recepção e os quatro tablets de professor lado a lado.
- **Recepção:** buscar um aluno pelo nome ou matrícula e registrar a chegada.
- **Tablet do professor:** aluno novo destacado com aviso sonoro, contador de alunos e faixa de sobrecarga acima de seis.
- **Ficha digital:** exercícios do dia, carga anterior, finalizar treino e registrar presença.
- **Alunos:** histórico de cada aluno, frequência e fichas vencendo.
- **Treinos:** montagem dos modelos de treino e da ficha do aluno.
- **Dashboard:** atendimentos por professor, horários de pico e alunos sem frequentar.

Abra o link em duas abas ou em dois aparelhos ao mesmo tempo: o que for feito em um aparece no outro, como aconteceria entre os tablets da academia.

O botão **Reiniciar** devolve a demonstração ao estado inicial antes de cada apresentação.

## Notas técnicas

- Arquivo único, sem dependências além das fontes do Google Fonts.
- A sincronização entre abas usa `BroadcastChannel` e funciona no mesmo navegador. Por isso o protótipo deve ser aberto pelo link publicado, e não como arquivo local.
- Na versão de produção, a sincronização entre aparelhos diferentes passa a ser feita pelo Supabase.
