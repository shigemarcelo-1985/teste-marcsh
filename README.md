# Montador de Réguas

Ferramenta para montar fluxogramas de jornada de réguas de CRM (dias, canais, copies, variantes A/B e criativos) e exportar o resultado em PNG.

## Como usar
1. Abra o `index.html` no navegador (ou acesse pelo GitHub Pages).
2. **+ Nova régua** → preencha código, nome, funil, gatilho e saída.
3. **+ Dia** cria o próximo dia; clique no dia para mudar o número.
4. **+ Canal** embaixo de cada dia (E-mail, WhatsApp, SMS, Push).
5. Clique em um card para editar copy, CTA, variantes A/B e enviar o criativo.
6. **Exportar PNG** baixa o fluxograma sem os botões de edição.

## Onde os dados ficam
- Fora do claude.ai, tudo fica salvo **no navegador de quem usa** (IndexedDB). Outra pessoa não vê suas réguas.
- Para compartilhar ou fazer backup: **Backup JSON** baixa todas as réguas; **Importar JSON** carrega em outro navegador.
- Imagens são redimensionadas para até 1200px e guardadas junto da régua.

## Variáveis
`{{Name|Futuro aluno}}`, `{{1}}` e `{{Insc Curso|Técnico}}` aparecem como etiquetas (Nome do aluno, Curso inscrito). No WhatsApp, `*texto*` vira negrito.

## Dependências
Nenhuma instalação. Usa `html2canvas` (cdnjs) e fontes do Google Fonts.

## Privacidade
Não versione backups JSON com dados de alunos ou copies internas em repositórios públicos.
