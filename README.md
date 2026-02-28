# Product Requirement Document (PRD) revisado e refinado pelo Copilot – App Finangel de Organização de Finanças Pessoais

## Contexto
O aplicativo Finangel, como o próprio nome denota, será o anjo que vai cuidar das finanças pessoais e simplificar o controle financeiro pessoal por meio de:
- Conversas em linguagem natural (chat com o usuário).
- Captura automática de notificações de apps de bancos sobre débitos e créditos.

A proposta é eliminar a necessidade de formulários complexos ou planilhas, respeitando o Design Universal, para que qualquer pessoa consiga usar de forma intuitiva.

## Problema
Muitos usuários desistem de organizar suas finanças porque:
- Os apps exigem muita entrada manual.
- Há pouca personalização e interação natural.

O objetivo é oferecer uma experiência fluida, conversacional e automatizada, com recomendações práticas de economia num tom informal.

## Público-Alvo
- Pessoas que desejam começar a organizar suas finanças sem complicação.
- Usuários iniciantes que buscam praticidade e acessibilidade.

## Funcionalidades-Chave

1. Registrar gastos via chat em linguagem natural
Exemplo: Usuário digita no chat: "Finangel, comprei um lanche por R$ 18 ontem à noite."
O app interpreta: valor R$ 18, categoria Alimentação, data correspondente a ontem, e registra como gasto.

2. Capturar notificações de apps de bancos sobre débitos e créditos
Exemplo: Notificação do banco: "Compra aprovada no débito: R$ 45,00 - Restaurante XYZ"
O app detecta o tipo (débito), valor (R$ 45), sugere categoria (Alimentação) e registra automaticamente.

3. Classificar automaticamente as transações
Exemplo: Transação capturada: "Pix recebido de R$ 200,00 - João"
O app classifica como crédito, categoria Transferência recebida, e sugere: "Deseja marcar como pagamento de serviço?"

4. Definir e acompanhar metas financeiras
Exemplo: Usuário digita no chat: "Quero economizar R$ 500 até o fim do mês."
O app responde: "Meta criada! Você já economizou R$ 120. Faltam R$ 380. Continue assim!"

5. Receber dicas de economia do Agente Financeiro
Exemplo: Após detectar gastos altos com delivery, o app sugere: "Você gastou R$ 320 com delivery este mês. Que tal cozinhar em casa 2x por semana para economizar até R$ 150?"

6. Visualizar relatórios simples e personalizados
Exemplo: Usuário acessa a tela de relatórios e vê: extrato, gráfico de pizza com categorias de gastos, linha do tempo com evolução da economia, e destaque: "Você economizou 12% a mais que no mês anterior!"

## MVP – Plano de Entregas

### Telas Principais
- Tela de Conversa: interação com o Agente Financeiro.
- Tela de Transações: lista de gastos e entradas capturados.
- Tela de Metas: definição e acompanhamento de objetivos.
- Tela de Relatórios: extrato e gráficos simples e acessíveis.

Observação: em todas as telas, usar fundo claro e paleta de cores confortáveis aos olhos.

### Recursos Necessários
- Módulo de NLP (Processamento de Linguagem Natural) para interpretar mensagens.
- Serviço de captura de notificações do sistema operacional (Android/iOS).
- Motor de classificação automática de transações.
- Banco de dados local + sincronização opcional em nuvem.

### Validação Inicial
- Testes com usuários iniciantes para verificar clareza da conversa.
- Avaliar se a captura de notificações funciona de forma confiável.
- Medir satisfação com relatórios simples e dicas automáticas.

## Design Universal
- Interface com contraste adequado e fontes legíveis. Tela de fundo claro e paleta de cores que facilite a identificação de cada informação e de cada tela.
- Navegação simples, sem excesso de menus.
- Compatibilidade com leitores de tela e comandos por voz.
- Feedback visual e sonoro para cada ação.

## Captura de Notificações Bancárias – Explicação Didática
O app usa a API de Notificações do sistema operacional (Android Notification Listener ou equivalente no iOS).

Funcionamento:
1. O banco envia uma notificação (ex.: "Compra de R$ 50,00 no supermercado").
2. O sistema entrega essa notificação ao app.
3. O app lê o texto da notificação, sem acessar dados sensíveis.
4. O texto é processado para identificar se é débito ou crédito.
5. O valor e a categoria são extraídos automaticamente e registrados.

Resumo: o app não acessa diretamente o banco, apenas interpreta as mensagens que já aparecem na tela do celular. Isso garante segurança e simplicidade.

## Diferencial
- Experiência conversacional em vez de formulários.
- Automatização via notificações, reduzindo esforço manual.
- Inclusão e acessibilidade como pilares do design.


### 2. Explorando o Lovable na Prática

Com seu PRD pronto e revisado, é hora de colocar a IA em ação. Abra o Lovable, cole seu prompt completo e peça o plano inicial do MVP do seu aplicativo. Como o plano gratuito limita você a 5 interações por dia, seja estratégico:
- Faça perguntas diretas e construtivas, como “crie o fluxo de telas com base nas funcionalidades listadas” ou “gere uma versão resumida do plano de MVP”;
- Priorize clareza nas instruções para aproveitar ao máximo cada resposta;

Durante essa etapa, você pode orientar a IA para três entregas principais:
1. Agente Financeiro: defina o comportamento e o tom de voz de um consultor financeiro pessoal, alinhado ao público e objetivo do app.
2. Fluxo de Telas: peça à IA para gerar o fluxo conceitual de telas com base nas funcionalidades descritas no PRD, simulando a interação por conversa.
3. Plano de MVP: solicite um resumo das 5 funcionalidades principais, dos recursos necessários e um plano de validação inicial (como medir se o app cumpre seu propósito).

Após submeter o PRD ao Lovable, o app Finangel foi criado, consistindo de 5 telas:
<img width="929" height="546" alt="Finangel_print 5" src="https://github.com/user-attachments/assets/fd2d62d0-3d23-4fa7-a2a6-27109b85f3dc" />
<img width="916" height="554" alt="Finangel_print 4" src="https://github.com/user-attachments/assets/bc3cc288-16e6-4c83-937a-d425a50b728a" />
<img width="934" height="547" alt="Finangel_print 3" src="https://github.com/user-attachments/assets/06c92fc8-0433-420e-bf9b-36c61be2fe74" />
<img width="917" height="551" alt="Finangel_print 2" src="https://github.com/user-attachments/assets/6cb46228-9261-44a2-9f90-c329d06903d4" />
<img width="1103" height="682" alt="Finangel_print 1" src="https://github.com/user-attachments/assets/f4352e6a-a71b-4802-a5de-96da7694bdf4" />

### 3. Entregando o Desafio na DIO

Finalize seu projeto criando um **repositório no GitHub** (pode ser um **fork** deste).  
https://github.com/LidiaTF/dio-lab-vibe-coding-app-financas/edit/main/README.md

No README do seu repositório, inclua:

- Seu **prompt final** (PRD); inserido acima.
  
- Prints ou pequenos vídeos das interações com a IA: Não lembrei de fazer as prints durante o processo. As interações com o Copilot funcionaram perfeitamente. No Lovable, acabei utilizando todos os créditos, em parte por não conhecer muito a plataforma. Quando foi gerado o app, havia dois botões: um para validar o app e outro para conectar o backend. Não sabia que clicando em cada botão os créditos eram utilizados. Além disso, pedi ao Lovable para acrescentar um box de saldo na tela de transações. Com isso, zeraram meus créditos.
  
- Um resumo do que o seu **App de Finanças Pessoais** faz: Elevator Pitch criado pelo Copilot: Imagine um aplicativo que organiza suas finanças sem formulários complicados ou planilhas cansativas. Nosso app Finangel combina conversas em linguagem natural com a captura automática de notificações bancárias, registrando débitos e créditos de forma prática e segura. Ele classifica transações, ajuda a definir metas, oferece dicas personalizadas de economia e mostra relatórios simples e visuais. O diferencial está na experiência: você conversa com um “Agente Financeiro” que entende seu jeito de falar e transforma notificações do banco em registros automáticos. É acessível, inclusivo e pensado para iniciantes que querem começar a cuidar do dinheiro sem complicação. Em poucos minutos, você terá clareza sobre seus gastos, metas e oportunidades de economizar — tudo de forma natural, rápida e universal.
  
  - Uma breve **reflexão sobre o processo**:
  1. **O que funcionou bem?** O Copilot respondeu de forma eficaz às interações e gerou um PRD que considero excelente. 
  2. **O que não funcionou como o esperado?** No Lovable, a validação do app não correspondeu ao esperado. Não houve ação correspondente ao chat nas telas de Transações e de Metas. Foi preciso dar input direto em cada tela. Além disso, o valor de 50.000,00 inserido manualmente em Metas mudou para 50,00 na exibição. Não pude refinar isso porque se esgotaram os créditos no Lovable. 
  3. **O que aprendeu sobre conversar com IAs?** Aprendi que os prompts deverão ser mais detalhados, especificando melhor principalmente o mecanismo das funcionalidades, isto é, a interconexão entre o chat e cada tela de registro.
