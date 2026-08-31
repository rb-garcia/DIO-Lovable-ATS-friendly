# DIO-Lovable-ATS-friendly
DIO-Lovable-ATS-friendly

# Prompt Otimizado
Crie "JobMatch AI" — app de matchmaking de vagas + gerador de currículo ATS-friendly.

STACK/DESIGN:
- shadcn/ui, Tailwind
- Paleta: azul claro (#38BDF8 primário, #E0F2FE backgrounds), branco, texto slate-900
- Layout: sidebar de navegação + área de conteúdo

PÁGINAS:
1. Dashboard: score médio de match, vagas salvas, currículos gerados (cards com stats)
2. Perfil: form de dados do usuário (experiências, skills, formação, upload de currículo base)
3. Vagas: lista de vagas com % de match (badge colorido: verde >80, amarelo 50-80, vermelho <50), filtros por área/senioridade/local, busca
4. Detalhe da vaga: descrição, skills exigidas vs. skills do usuário (comparativo visual), botão "Gerar currículo ATS"
5. Gerador ATS: recebe vaga selecionada → cria versão do currículo otimizada com keywords da vaga, preview lado a lado (original vs. otimizado), score ATS estimado, export PDF
6. Histórico: currículos gerados por vaga, com data e score

LÓGICA DE MATCH:
- Comparar skills do perfil vs. requisitos da vaga (% de sobreposição)
- Peso: skills obrigatórias 60%, desejáveis 25%, senioridade 15%

DADOS: mock realista (10 vagas variadas, 1 perfil exemplo preenchido)

COMPONENTES shadcn: Card, Badge, Tabs, Dialog, Progress, Table, Input, Select
