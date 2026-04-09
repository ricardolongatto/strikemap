# StrikeMap — Pentest Intelligence Dashboard

Uma ferramenta **100% client-side** que roda direto no browser sem instalação, sem servidor, sem dependências. Abra o arquivo HTML e comece a operar.

---

## O que é

StrikeMap é um dashboard de inteligência para projetos de pentest. Ele foi criado para substituir blocos de notas e planilhas durante a execução de um projeto real, centralizando em um único lugar:

- O rastreamento das fases do pentest (recon → análise → exploração → entrega)
- O mapeamento de subdomínios e sistemas ativos
- O registro de endpoints descobertos
- O registro e classificação de vulnerabilidades (com CVSS)
- A cadeia de ataque (attack chain) visual
- Notas em Markdown com suporte a screenshots colados
- Mapa interativo de hosts (canvas drag-and-drop)
- Escopo e informações do projeto

Tudo salvo no `localStorage` do browser, sem nenhum dado enviado para servidor.

---

## Como usar

1. Faça o download do arquivo `strikemap-v1.html`
2. Abra no browser (Chrome ou Firefox recomendado)
3. Clique em **+ Novo projeto** e preencha os dados do escopo
4. Navegue pelas abas conforme avança no pentest

Não precisa de internet após o download. Funciona offline.

---

## Funcionalidades

| Módulo | O que faz |
|---|---|
| **Fases** | Acompanha o progresso do projeto por etapa, com subtarefas customizáveis |
| **Subdomínios** | Registra hosts descobertos, IPs, tecnologias e status (ativo, vulnerável, comprometido…) |
| **Sistemas** | Mapeia serviços e portas abertas |
| **Endpoints** | Cataloga paths descobertos com método HTTP, status code e flag (normal / interessante / explorado) |
| **Vulnerabilidades** | Registra findings com severidade, CVSS, evidências e PoC |
| **Attack Chain** | Visualiza a sequência de eventos de ataque em fluxo linear |
| **Mapa** | Canvas interativo dos hosts com status visual em tempo real |
| **Notas** | Editor Markdown com preview ao lado e suporte a Ctrl+V de screenshots |
| **Escopo** | Exibe as informações do projeto, in-scope e out-of-scope |

---

## Importação e exportação

- **Exportar JSON** — backup completo do projeto
- **Importar JSON** — restaura um backup
- **Exportar Markdown** — gera um relatório em texto estruturado
- **Importação de ferramentas** — suporte a formatos de saída de ferramentas comuns de recon (auto-detect)

---

## Filosofia

A ferramenta foi construída com a metodologia da Desec em mente, dividindo o projeto em três grandes blocos:

```
Mapeamento da Superfície de Ataque → Análise de Segurança → Resultados
```

O StrikeMap acompanha o pentester do início ao fim, sem atrapalhar o fluxo de trabalho.

---

## Tecnologia

- HTML + CSS + JavaScript vanilla
- Zero dependências externas
- Zero backend
- Dados persistidos via `localStorage`
- Compatível com qualquer browser moderno

---

## Licença

Distribuído gratuitamente para uso educacional e profissional.  
Proibida a redistribuição com alteração de autoria.

---

<div align="center">
  <strong>StrikeMap</strong> · Idealizado por <strong>Ricardo Longatto</strong> · <a href="https://desecsecurity.com">Desec Security</a><br>
  <em>Pentest com método. Resultado com impacto.</em>
</div>
