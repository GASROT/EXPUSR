# FATEC Carreiras

A plataforma **FATEC Carreiras** atua como uma ponte inteligente entre o talento acadêmico (estudantes da FATEC) e as necessidades reais do mercado (empresas parceiras). O projeto busca reduzir o abismo entre currículos e vagas através de um *Matchmaker Dinâmico*, permitindo um recrutamento mais assertivo e oferecendo feedbacks focados no desenvolvimento dos alunos.

## Acesso (Exemplo)
🔗 [Vercel](https://fatec-carreiras-example.vercel.app)

## Material aplicado ao projeto: Processos PD (Espaco do Problema) - Portfolio

Os processos de Product Discovery foram aplicados diretamente na interface principal do projeto (`index.html`), com secoes dedicadas para analise do Espaco do Problema.

Aplicacoes implementadas:

1. Briefing do problema (Mission Briefing adaptado).
2. Metodo 5W1H para sintese do problema.
3. Definicao de personas (primaria e secundarias).
4. Matriz CSD para validacao de requisitos.
5. Mapa de Jornada para identificar friccoes.
6. Estrutura de entregavel para portfolio ("O Desafio e o Contexto").
7. Riscos de Discovery e checklist de prontidao antes da ideacao.

---

## Pesquisa: Heuristicas de Usabilidade e Fatores Humanos

Esta pesquisa resume como aplicar heuristicas de usabilidade em software interativo com foco em interfaces para pessoas com deficiencia.

Em termos praticos, este material funciona como um guia de decisao para o time: ajuda a transformar principios abstratos de UX e acessibilidade em criterios objetivos de projeto, desenvolvimento e validacao.

Como ler a pesquisa:

1. Secoes 1 a 4: entendimento conceitual (o que e, para que serve, onde e quando aplicar).
2. Secao 5: metodo operacional para executar no dia a dia.
3. Secoes 6 a 8: resultados esperados, traducao para briefing e direcionamento estrategico.
4. Secao 9: base de referencia tecnica e normativa para fundamentar decisoes.

## 1) O que sao heuristicas de usabilidade

Heuristicas de usabilidade sao principios praticos para avaliar e melhorar interfaces. Elas funcionam como um "checklist de qualidade da experiencia", ajudando a identificar problemas antes de virar retrabalho.

Em uma equipe de produto, heuristicas nao substituem testes com usuarios, mas aceleram a deteccao inicial de problemas de fluxo, linguagem, consistencia visual e feedback do sistema. Isso reduz custo de correcao nas fases finais.

As 10 heuristicas de Nielsen (referencia classica) sao:

1. Visibilidade do status do sistema.
2. Correspondencia entre sistema e mundo real.
3. Controle e liberdade do usuario.
4. Consistencia e padroes.
5. Prevencao de erros.
6. Reconhecimento em vez de memorizacao.
7. Flexibilidade e eficiencia de uso.
8. Design estetico e minimalista.
9. Ajudar a reconhecer, diagnosticar e recuperar erros.
10. Ajuda e documentacao.

## 2) Para que servem

No contexto do FATEC Carreiras, elas servem para:

Esses pontos existem para garantir que a plataforma seja eficiente para quem usa e sustentavel para quem opera. Na pratica, isso significa menos friccao para estudantes, melhor qualidade de triagem para empresas e menos retrabalho para o time tecnico.

1. Reduzir barreiras de uso para estudantes, recrutadores e administradores.
2. Aumentar a taxa de conclusao de tarefas criticas (cadastro, candidatura, feedback).
3. Diminuir erros de formulario e abandono de fluxo.
4. Tornar a plataforma mais inclusiva para pessoas com deficiencia visual, auditiva, motora e cognitiva.
5. Padronizar decisoes de UX para futuras incrementacoes.

## 3) Onde aplicar no projeto

Aplicar em toda jornada principal:

Aplicar "em toda jornada" significa revisar cada tela que impacta decisao do usuario, envio de dados ou acompanhamento de status. Em fluxos longos (como candidatura), pequenos problemas acumulados aumentam abandono.

1. Landing e descoberta de vagas.
2. Cadastro e login.
3. Perfil do estudante (curriculo, competencias, portfolio).
4. Publicacao e gestao de vagas pelas empresas.
5. Processo de candidatura e acompanhamento de status.
6. Feedback orientado a desenvolvimento.
7. Painel administrativo e relatorios.

## 4) Quando usar

Usar heuristicas e criterios de acessibilidade em ciclos continuos:

A aplicacao continua evita o erro comum de tratar acessibilidade apenas no fim. Quanto antes os criterios entram no ciclo, menor o custo de ajuste e maior a chance de manter consistencia entre modulos.

1. Antes do desenvolvimento: refinamento de requisitos e prototipos.
2. Durante o desenvolvimento: revisoes de tela e validacoes por historia.
3. Antes de release: avaliacao heuristica + checklist WCAG.
4. Depois da release: monitoramento de metricas e ajustes evolutivos.

## 5) Como usar (metodo pratico)

Esta secao converte principios em operacao. O objetivo e sair de uma analise subjetiva ("a tela parece boa") para uma avaliacao rastreavel, com severidade, prioridade e evidencias de melhoria.

### 5.1 Fluxo recomendado

1. Selecionar fluxo critico (ex.: candidatura em vaga).
2. Executar avaliacao heuristica com 3 a 5 avaliadores.
3. Classificar severidade de cada problema (0 a 4):
	- 0: nao e problema
	- 1: cosmetico
	- 2: baixo
	- 3: alto
	- 4: critico
4. Mapear cada problema para criterio de acessibilidade (WCAG 2.2).
5. Criar acoes no backlog com prioridade por impacto x esforco.
6. Validar correcao com testes de usabilidade (incluindo PCD).

### 5.2 Heuristicas + acessibilidade (exemplos aplicaveis)

A tabela abaixo mostra como conectar problema de UX com criterio tecnico de acessibilidade. Essa ligacao facilita priorizacao no backlog e evita correcoes isoladas sem impacto real para o usuario.

| Heuristica | Risco comum no contexto | Ajuste recomendado | Criterio de acessibilidade relacionado |
|---|---|---|---|
| Visibilidade do status | Usuario nao sabe se candidatura foi enviada | Confirmacao clara + status da candidatura em timeline | WCAG 2.2 - 4.1.3 Status Messages |
| Controle e liberdade | Dificuldade para desfazer acao | Botao "voltar", "editar" e "cancelar" com confirmacao | WCAG 2.2 - 3.2.2 On Input |
| Prevencao de erros | Formulario extenso com envio invalido | Validacao em tempo real, mascaras e exemplos | WCAG 2.2 - 3.3.1 / 3.3.3 |
| Reconhecimento vs memorizacao | Usuario precisa lembrar codigos/etapas | Labels claros, placeholders de apoio, historico visivel | WCAG 2.2 - 2.4.6 Headings and Labels |
| Flexibilidade e eficiencia | Navegacao lenta sem atalho | Ordem de tab logica, atalhos de teclado, autosave | WCAG 2.2 - 2.1.1 Keyboard |

### 5.3 Requisitos minimos para interfaces inclusivas

Esses requisitos devem ser tratados como baseline de qualidade, nao como diferencial opcional. Se um deles falha, parte dos usuarios perde autonomia de uso.

1. Navegacao completa por teclado.
2. Contraste adequado de texto e componentes.
3. Estrutura semantica correta (titulos, landmarks, labels).
4. Textos alternativos em imagens relevantes.
5. Mensagens de erro claras, com orientacao de correcao.
6. Feedbacks nao dependentes apenas de cor/icone.
7. Compatibilidade com leitores de tela.
8. Conteudo multimidia com legenda e, quando necessario, transcricao.

## 6) Resultados esperados

Resultados esperados apos aplicar o processo:

Os resultados abaixo devem ser acompanhados por serie historica (por sprint ou release), para comprovar evolucao real e orientar novas prioridades de UX e engenharia.

1. Aumento da taxa de conclusao dos fluxos principais.
2. Reducao de erros por formulario e tickets de suporte.
3. Reducao de abandono em cadastro e candidatura.
4. Melhor percepcao de clareza, confianca e autonomia do usuario.
5. Evolucao da conformidade com WCAG 2.2 em cada release.

### Indicadores sugeridos (para acompanhar evolucao)

1. Taxa de conclusao de tarefa por perfil de usuario.
2. Tempo medio para concluir candidatura.
3. Taxa de erro por campo de formulario.
4. Taxa de abandono por etapa do funil.
5. Quantidade de problemas de severidade 3 e 4 por release.
6. Percentual de criterios WCAG atendidos por modulo.

## 7) Como usar esta pesquisa para atualizar o briefing do projeto

Nesta etapa, a pesquisa deixa de ser apenas referencia teorica e passa a virar contrato de qualidade do produto. Ou seja: o briefing passa a explicitar o que deve ser entregue e como sera validado.

### 7.1 Blocos que devem entrar no briefing

1. Objetivo de UX e acessibilidade:
	- "Garantir experiencia inclusiva e eficiente para estudantes e empresas, com foco em acessibilidade digital e reducao de friccao nos fluxos criticos."
2. Publicos e necessidades especificas:
	- Incluir explicitamente pessoas com deficiencia visual, auditiva, motora e cognitiva.
3. Requisitos funcionais e nao funcionais:
	- Adicionar criterios de teclado, contraste, semantica, feedback e tolerancia a erro.
4. Criterios de aceite por historia:
	- Toda historia deve ter validacao heuristica e criterio minimo de acessibilidade.
5. Metricas de sucesso:
	- Definir metas trimestrais para conclusao, erro e abandono.

### 7.2 Template rapido para historias (futuras incrementacoes)

Use este padrao em cada nova funcionalidade:

1. Objetivo da funcionalidade.
2. Fluxo principal e fluxos alternativos.
3. Heuristicas impactadas (listar quais das 10).
4. Criterios WCAG aplicaveis.
5. Riscos de usabilidade identificados.
6. Criterios de aceite (funcional + acessibilidade + usabilidade).
7. Metricas para monitoramento apos release.

### 7.3 Prioridade inicial de backlog (sugestao)

1. Padronizar formularios (labels, erros, ajuda contextual, tabulacao).
2. Revisar navegacao por teclado em todos os fluxos criticos.
3. Implementar padrao unico de mensagens de status e erro.
4. Ajustar contraste e hierarquia visual em componentes base.
5. Incluir testes com usuarios, incluindo pessoas com deficiencia.

## 8) Briefing v2 (com melhorias da revisao da v1)

Esta versao consolida os ajustes sugeridos no feedback da v1, principalmente em clareza de escopo, acessibilidade, criterios objetivos de qualidade e estrategia de evolucao do produto.

Interpretacao recomendada: use este briefing como base de priorizacao de backlog, definicao de criterios de aceite e alinhamento entre produto, design e desenvolvimento.

### 8.1 Visao do produto

O FATEC Carreiras e uma plataforma de conexao entre estudantes e empresas parceiras, com foco em reduzir ruido na triagem, elevar a qualidade de candidatura e apoiar desenvolvimento profissional com feedback orientado.

### 8.2 Problema central (redefinido)

1. Estudantes candidatam-se sem sinal claro de aderencia e sem feedback acionavel.
2. Empresas recebem alto volume de perfis pouco aderentes, com custo de triagem elevado.
3. Barreiras de usabilidade e acessibilidade reduzem conversao e inclusao digital.

### 8.3 Objetivos estrategicos

1. Melhorar o match entre perfil academico-tecnico e vaga.
2. Reduzir tempo e esforco de triagem para recrutadores.
3. Garantir experiencia inclusiva para pessoas com deficiencia.
4. Gerar feedback pratico para evolucao de competencias dos estudantes.

### 8.4 Publicos e necessidades

1. Estudante:
	- Entender aderencia a vaga antes de candidatar.
	- Receber feedback objetivo de lacunas tecnicas/comportamentais.
	- Navegar com autonomia por teclado, leitor de tela e linguagem clara.
2. Recrutador:
	- Publicar vaga com requisitos realistas e padronizados.
	- Receber candidatos ranqueados por compatibilidade.
	- Filtrar com rapidez sem perder candidatos promissores.
3. Administracao/gestao academica:
	- Acompanhar indicadores de empregabilidade e lacunas de formacao.

### 8.5 Proposta de valor v2

1. Matchmaker Dinamico com transparencia de criterios.
2. Indice de Compatibilidade por vaga e por candidato.
3. Feedback Automatizado com sugestoes de trilhas de melhoria.
4. Jornada com requisitos minimos de acessibilidade desde o MVP.

### 8.6 Escopo funcional (MVP v2)

1. Cadastro/login e perfil completo do estudante (habilidades, projetos, experiencias).
2. Cadastro e publicacao de vagas com formulario guiado por senioridade.
3. Motor de matching com score e explicacao resumida dos fatores de aderencia.
4. Painel de candidaturas com status visivel e historico.
5. Feedback automatizado para candidatos nao selecionados.
6. Painel do recrutador com ranking e filtros essenciais.

### 8.7 Requisitos nao funcionais (novos criterios v2)

1. Usabilidade:
	- Aplicacao das 10 heuristicas de Nielsen nas telas criticas.
2. Acessibilidade:
	- Atendimento progressivo a WCAG 2.2 nivel AA nos fluxos principais.
	- Navegacao completa por teclado.
	- Contraste e semantica adequados.
	- Feedback de erro e status compreensivel para tecnologias assistivas.
3. Desempenho:
	- Tempo de resposta adequado para busca/listagem em condicoes padrao.
4. Confiabilidade:
	- Historico de status de candidatura consistente e auditavel.

### 8.8 Criterios de aceite por incremento

Cada entrega deve conter:

1. Validacao funcional do fluxo principal e fluxo alternativo.
2. Checklist heuristico com problemas classificados por severidade (0 a 4).
3. Checklist de acessibilidade aplicado ao escopo da historia.
4. Evidencia de teste com usuario (quando possivel, incluindo PCD).
5. Plano de monitoramento pos-release com metricas definidas.

### 8.9 KPIs e metas iniciais

1. Aumentar taxa de conclusao de candidatura.
2. Reduzir taxa de abandono nas etapas de cadastro e candidatura.
3. Reduzir erros de formulario por sessao.
4. Reduzir volume de triagem manual de baixa aderencia.
5. Aumentar percentual de conformidade WCAG no escopo implementado.

### 8.10 Roadmap de evolucao (3 ondas)

1. Onda 1 - Fundacao:
	- Formularios acessiveis, padrao de mensagens de erro/status, fluxo basico de candidatura.
2. Onda 2 - Inteligencia:
	- Melhorias no algoritmo de match, explicabilidade do score e feedback enriquecido.
3. Onda 3 - Escala e governanca:
	- Analytics de empregabilidade, painel de indicadores institucionais e ciclo continuo de melhoria UX.

### 8.11 Riscos e mitigacoes

1. Risco: score opaco gerar desconfiança.
	- Mitigacao: exibir fatores de aderencia e lacunas de forma clara.
2. Risco: requisitos de vagas irreais.
	- Mitigacao: formulario guiado e validacoes de consistencia por senioridade.
3. Risco: baixa adesao por barreiras de acessibilidade.
	- Mitigacao: WCAG no criterio de aceite e testes com usuarios diversos.

### 8.12 Definicao de pronto (DoR/DoD simplificada)

1. Historia entra em desenvolvimento somente com heuristicas impactadas e criterios WCAG mapeados.
2. Historia e considerada pronta apenas com validacao funcional + heuristica + acessibilidade.
3. Historia e monitorada por KPI definido ate o ciclo seguinte.

## 9) Fontes

1. Nielsen Norman Group. 10 Usability Heuristics for User Interface Design.
	- https://www.nngroup.com/articles/ten-usability-heuristics/
2. W3C. Web Content Accessibility Guidelines (WCAG) 2.2.
	- https://www.w3.org/TR/WCAG22/
3. W3C WAI. How to Meet WCAG (Quick Reference).
	- https://www.w3.org/WAI/WCAG22/quickref/
4. ISO 9241-210:2019. Ergonomics of human-system interaction - Human-centred design for interactive systems.
	- https://www.iso.org/standard/77520.html
5. Governo Federal (Brasil). eMAG - Modelo de Acessibilidade em Governo Eletronico.
	- https://emag.governoeletronico.gov.br/
6. Brasil. Lei Brasileira de Inclusao (Lei no 13.146/2015).
	- http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13146.htm
