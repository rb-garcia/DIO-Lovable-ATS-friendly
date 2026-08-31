# DIO-Lovable-ATS-friendly
DIO-Lovable-ATS-friendly

# Prompt Otimizado
Crie "JobMatch AI" — app de matchmaking de vagas + gerador de currículo ATS-friendly.

## Stack/Design:
- shadcn/ui, Tailwind
- Paleta: azul claro (#38BDF8 primário, #E0F2FE backgrounds), branco, texto slate-900
- Layout: sidebar de navegação + área de conteúdo

## Páginas:
1. Dashboard: score médio de match, vagas salvas, currículos gerados (cards com stats)
2. Perfil: form de dados do usuário (experiências, skills, formação, upload de currículo base)
3. Vagas: lista de vagas com % de match (badge colorido: verde >80, amarelo 50-80, vermelho <50), filtros por área/senioridade/local, busca
4. Detalhe da vaga: descrição, skills exigidas vs. skills do usuário (comparativo visual), botão "Gerar currículo ATS"
5. Gerador ATS: recebe vaga selecionada → cria versão do currículo otimizada com keywords da vaga, preview lado a lado (original vs. otimizado), score ATS estimado, export PDF
6. Histórico: currículos gerados por vaga, com data e score

## Lógica de Match:
- Comparar skills do perfil vs. requisitos da vaga (% de sobreposição)
- Peso: skills obrigatórias 60%, desejáveis 25%, senioridade 15%

Dados: mock realista (10 vagas variadas, 1 perfil exemplo preenchido)

Componentes shadcn: Card, Badge, Tabs, Dialog, Progress, Table, Input, Select

# Resumo ATS Friendly
Contexto: desenvolvimento de um app de matchmaking de vagas com gerador de currículos ATS-friendly, usando Lovable como plataforma de construção via prompts em linguagem natural, com shadcn/ui e paleta azul claro/branco.

- Dashboard — score médio de match em indicador radial, contadores de vagas salvas e currículos, top 3 recomendações e timeline de atividade.
- Vagas — 10 vagas realistas com badge colorido de match (verde >80%, amarelo 50–80%, vermelho <50%), busca e filtros por área, senioridade e localização.
- Detalhe da vaga — comparativo visual de skills (você vs. vaga), breakdown com os pesos 60/25/15 e botão "Gerar currículo ATS".
- Gerador ATS — animação de análise, preview lado a lado (original vs. otimizado com keywords destacadas), score ATS estimado e exportação em PDF.
- Perfil — form completo com experiências, skills hard/soft, senioridade e upload de currículo base.
- Histórico — tabela dos currículos gerados por vaga, com data e score.

# Processo
## O que funcionou bem?
- Prompt inicial estruturado reduziu o retrabalho
- Uso de componentes shadcn manteve a consistência visual sem correções

## O que não funcionou como o esperado?
- A logica de match interpretada de forma simplificada
- Preview lado a lado do curriculo
- Export PDF, formato

## O que aprendeu sobre conversar com IAs?
- Especificidade vale mais que extensão
- A IA não infere regras de negócio, ela inventa
- Ambiguidade visual é a maior fonte de retrabalho
- Iterar é parte do processo

# Telas
<img width="1293" height="828" alt="image" src="https://github.com/user-attachments/assets/0d68e5c0-01a0-402e-9535-2a5a3e6b7a73" />

<img width="1299" height="829" alt="image" src="https://github.com/user-attachments/assets/6990b1b4-ebfd-4391-8cfd-1491f5416278" />

<img width="1302" height="832" alt="image" src="https://github.com/user-attachments/assets/527cfc31-1af8-4767-80fa-b213bcf47b13" />
