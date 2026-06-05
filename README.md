# Guia de Segurança no Desenvolvimento de Software

> Artefato web desenvolvido como produto técnico do Trabalho de Conclusão de Curso "Diretrizes de Segurança para Desenvolvedores de Aplicativos do Governo Federal" de Julia Knabem, pela Universidade Federal de Santa Catarina (UFSC), 2026.

---

## Sobre o projeto

Este repositório contém o código-fonte do **Guia de Segurança no Desenvolvimento de Aplicativos Governamentais**, uma aplicação web que organiza diretrizes práticas de segurança por etapa do ciclo de vida de desenvolvimento de software (SDLC). O guia foi construído como produto técnico do TCC e tem como objetivo auxiliar desenvolvedores, especialmente os que atuam em contextos governamentais, a incorporar práticas de segurança desde as fases iniciais do desenvolvimento.

As diretrizes foram selecionadas a partir de uma análise comparativa de normas, frameworks e legislação vigente, priorizadas por impacto, aplicabilidade ao SDLC, relevância normativa e adequação ao contexto de aplicativos governamentais brasileiros.

---

## Estrutura de arquivos

```
.
└── index.html   # Aplicação completa (HTML + CSS + JS em arquivo único)
```

O guia foi implementado como um único arquivo HTML autocontido, sem dependências de build ou frameworks JavaScript externos. Todo o estilo e a lógica de navegação estão embutidos no próprio arquivo.

---

## Como usar

O guia está publicado e acessível diretamente pelo navegador, sem necessidade de instalação:

🔗 **[Acessar o guia](https://juliaknabem.github.io/diretrizes-seguranca-para-desenvolvedores/)**

Por ser uma aplicação estática de arquivo único, também é possível rodá-lo localmente clonando o repositório:

```bash
git clone https://github.com/juliaknabem/diretrizes-seguranca-para-desenvolvedores.git
cd guia-seguranca-sdlc
```

Em seguida, abra o `index.html` diretamente no navegador ou sirva localmente para evitar eventuais restrições de CORS com fontes externas:

```bash
# Com Node.js
npx serve .

# Com Python
python3 -m http.server 8080
```

Não há instalação de dependências, processo de build ou configuração necessária.

---

## Como contribuir

Este projeto é open source e contribuições são bem-vindas, seja para corrigir informações, adicionar novas diretrizes, melhorar a interface ou apontar fontes complementares.

**Antes de contribuir, leia:**
- As diretrizes do guia devem ser sempre embasadas em pelo menos uma das fontes normativas listadas na seção [Fontes normativas](#fontes-normativas).
- Por ser um artefato acadêmico, alterações que modifiquem o escopo ou a metodologia do guia devem ser discutidas em uma issue antes de qualquer pull request.

**Fluxo de contribuição:**

1. Abra uma [issue](https://github.com/juliaknabem/diretrizes-seguranca-para-desenvolvedores/issues) descrevendo o que deseja alterar ou adicionar e por quê.
2. Caso a issue seja aprovada, faça um fork do repositório e crie uma branch com um nome descritivo:
   ```bash
   git checkout -b melhoria/nome-da-alteracao
   ```
3. Faça as alterações no `index.html` e verifique o resultado abrindo o arquivo no navegador.
4. Abra um pull request para a branch `main`, descrevendo o que foi alterado e referenciando a issue correspondente.

**Tipos de contribuição bem-vindos:**
- Correção de informações desatualizadas ou imprecisas
- Adição de diretrizes com embasamento normativo
- Melhoria de acessibilidade (contraste, navegação por teclado, leitores de tela)
- Correções de ortografia e clareza nos textos
- Ajustes de responsividade para dispositivos móveis

**Tipos de contribuição que não serão aceitos:**
- Diretrizes sem referência a normas, frameworks ou legislação reconhecidos
- Alterações que removam as referências normativas existentes
- Adição de dependências externas (o projeto mantém intencionalmente zero dependências de build)

---

## Funcionalidades

O guia é organizado em três níveis de navegação:

**Nível 1 — Mapa do SDLC**
Visão geral das etapas do ciclo de vida de desenvolvimento cobertas pelo guia:
- Requisitos
- Projeto
- Codificação
- Testes
- Implantação e manutenção

**Nível 2 — Painel da etapa**
Ao selecionar uma etapa, são listadas as diretrizes de segurança aplicáveis àquela fase, com indicação das fontes normativas que embasam cada diretriz.

**Nível 3 — Detalhe da diretriz**
Cada diretriz pode ser expandida para exibir descrição completa, justificativa, referências normativas e exemplos práticos de aplicação.

**Seções complementares:**
- **Cobertura frente ao OWASP Top 10 (2025):** mapeamento das diretrizes do guia às dez categorias de vulnerabilidade mais críticas, com indicação de cobertura total, parcial ou não cobertura.
- **Fontes utilizadas:** lista completa das normas, frameworks e legislação que fundamentam o guia, com links para os documentos originais.

---

## Fontes normativas

As diretrizes do guia são fundamentadas nas seguintes referências:

| Sigla | Documento |
|---|---|
| LGPD | Lei nº 13.709/2018 — Lei Geral de Proteção de Dados Pessoais |
| ISO 27001 | ABNT NBR ISO/IEC 27001:2022 — Segurança da informação |
| NIST CSF | NIST Cybersecurity Framework 2.0 (2024) |
| OWASP SCP | OWASP Secure Coding Practices v2.0.1 |
| OWASP SbD | OWASP Secure by Design Framework v0.5 (2025) |
| OWASP Top 10 | OWASP Top 10 — 2025 |
| OWASP ASVS | OWASP ASVS v5.0.0 (2025) |
| PPSI | Guia de Requisitos Mínimos de Privacidade e Segurança — SGD/MGI |
| PSI | Guia do Framework de Privacidade e Segurança da Informação — SGD/MGI |
| TCU | Boas Práticas de Segurança da Informação — TCU |

---

## Licença

Este projeto foi desenvolvido para fins acadêmicos. Os documentos de referência utilizados (OWASP, NIST, ISO, LGPD, guias do Governo Federal) são de titularidade de seus respectivos autores e organizações, e estão citados com os devidos créditos na seção "Fontes utilizadas" do próprio guia.
