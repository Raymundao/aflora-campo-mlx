# Aflora Campo — Roadmap / Backlog

> Lista do que falta fazer e ideias futuras. Atualizada conforme a gente avança.

## ✅ Feito (v11–v18)
- v11 — renomeado "Aflora Campo" (nome + ícone + metas iOS)
- v12 — GPS iOS (re-arma watch, erro visível, wake lock); nome de espécie propaga (censo + parcelas + herbáceo); teclado da placa 123/ABC
- v13 — voltar do Android navega entre telas (não fecha o app); fotos de parcela herbácea sem subdivisão
- v14 — foto de espécie no censo + "onde ocorre" (parcela/censo + placas) na aba Espécies; botões 🗂️ Camadas / 📥 Importar / 📤 Exportar (com seletor)
- v15 — wizard "o que você vai fazer?" ao criar projeto
- v16 — controle de acesso por código com validade (grandfather pro time) + gerar-codigo.html
- v17 — cache do "baixar área offline" alinhado com o SW
- v18 — config por módulo (censo esconde parcela/erro); classe de uso do solo "Árvores isoladas"; botão "Salvar e ir pro projeto"; ⚙ discreto no card; abas por módulo; nome custom por estrato; "sem estágio" some
- **Guias PDF** — "Guia rápido" (instalar + 1º censo, iPhone/Android) e "Tutorial completo" (módulos + cada botão do mapa de censo + link Espécies↔Censo/Parcelas)

## 🔧 A fazer — features
- **Teclado CAP/altura**: Enter avança + seta ↓ na tela que **não fecha o teclado** (fluxo "todos os CAPs, depois as alturas").
- **Export — compartilhar**: opção de **Compartilhar** (Web Share → WhatsApp/Drive) além de baixar, pra escolher onde salvar.
- **Lista mestra de espécies**: (app) pré-carregar lista grande só no autocomplete, sem poluir a aba Espécies; (dados) garimpar ~150-200 relatórios da pasta de consultorias e unificar numa tabela-mestra.
- **Campos de formulário customizáveis**: default CAP+Altura, e o usuário adiciona campos (altura comercial, epífitas, qualidade de fuste…). Vale mais pras parcelas.
- **Plano de lançamento**: site com prints/vídeos por módulo + tabela de preços + modelo de créditos/day-pass + estratégia UFJF (projeto/extensão vs contrato de manutenção, sem virar produto do laboratório).

## 🧩 Módulos futuros (pedidos)
- **Módulo financeiro**: tirar foto + anotar dados de notas de pagamento de despesas de campo; exportar tudo num XLSX já certinho, linkando fotos + informações.
- **Módulo de monitoramento**: importar um Excel de campo de parcelas **já existentes**; opção de pegar novos dados de **indivíduos recrutas**; marcar indivíduo **morto** ou **não encontrado**.

## 🚀 Grandes ideias / visão
- **Desenho inteligente de fitofisionomias (corte automático de interseção)**: ao desenhar um polígono dentro da **ADA** que sobrepõe outro já desenhado, **cortar a interseção automaticamente** (sem áreas sobrepostas). Cuidado em **separar o que é ADA** do que é **polígono de fitofisionomia**. (Conecta com a metodologia `app-desenhar-fitos.md` e o pacote `aflora_tools.mapas`.)
- **Prováveis ocorrências por região (REFLORA/GBIF + meu banco)**: ao iniciar um projeto numa região de MG (Zona da Mata, Triângulo, Norte…), gerar uma **lista das espécies esperadas** — principalmente as **ameaçadas** — cruzando **REFLORA/GBIF** com o **banco dos meus inventários** (pasta de consultorias). Ajuda quem vai a campo numa área desconhecida. A princípio só **MG**. (Liga com a "lista mestra de espécies" acima.)
- **Gerar o relatório no próprio app** *(objetivo final)*: a partir dos dados de campo, produzir o relatório (lista florística, fitossociologia, volume, etc.) direto no app — reaproveitando os pipelines do `aflora_tools`.

## 🧭 Decisões / testes do Diego
- **Privacidade/hospedagem**: deixar repos privados + mover hospedagem (Cloudflare grátis → link novo, ou GitHub Pro US$4/mês → mesmo link) + trocar o link `-mlx`.
- **Testar no aparelho**: July confirmar GPS no iPhone; validar v13–v18 no campo (voltar do Android, wizard, validade, config por módulo).

## ⚠️ Riscos pré-existentes (anotados)
- Form de ponto do censo **não auto-salva** enquanto digita (só ao tocar Salvar). Dá pra fazer auto-salvar como nas parcelas.
- Update do app recarrega — se pegar um form aberto sem salvar, perde.

## 🗂️ Housekeeping
- App de campo **Leaflet** (não-GPU) ficou em versão antiga; migrado pro GLX (MapLibre) → decidir arquivar.
- Botões antigos de export na lista de pontos (lst-kmz/lst-xlsx) redundantes com o novo 📤 — remover.
- Rodar o **"salva tudo"** (memória/Obsidian/Linear) da maratona (códigos de acesso, decisões, roadmap).
