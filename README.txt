# EcoBag+ — Landing Page (estática)

Este pacote contém uma landing page simples (HTML/CSS) para validar o MVP do **EcoBag+**.

## Como usar
1. Crie **dois Google Forms** (um para *Consumidor* e outro para *Supermercado*).
   - Clique em **Enviar** > ícone `<>` (Incorporar HTML) > copie a **URL** do `src`.
2. No arquivo `index.html`, procure por:
   ```js
   const urls = {
     consumidor: "https://docs.google.com/forms/d/e/SEU_ID_FORM_CONSUMIDOR/viewform?embedded=true",
     supermercado: "https://docs.google.com/forms/d/e/SEU_ID_FORM_SUPERMERCADO/viewform?embedded=true"
   };
   ```
   e substitua pelas URLs de incorporação reais.
3. Publique a pasta em um hosting estático (Netlify, Vercel, GitHub Pages, ou **Wix**/RDStation via bloco HTML).
4. Divulgue o **link publicado** com UTM parameters, por ex.:  
   `https://seu-dominio.site/?utm_source=whatsapp&utm_campaign=piloto`

## Medição básica
- Use relatórios do Google Forms + planilha sincronizada para ver contagens de respostas.
- Registre os **UTMs** (dica: adicione um campo de pergunta “Como conheceu?” para conciliar).
- Métricas principais:
  - **Visitas (V)**: page views (Netlify/Vercel Analytics) ou cliques únicos no Bitly.
  - **Leads (L)**: envios válidos do(s) formulário(s).
  - **Conversão (CR)** = `L / V`.
  - **Custo por lead (CPL)** = `gasto total mídia / L` (se houver).

## Editar textos/estilo
- Edite as seções em `index.html` e o visual em `styles.css`.
- O site é *mobile-first* e não usa bibliotecas externas além da fonte Google.

## LGPD
Incluímos um bloco de privacidade no FAQ. No Google Forms, adicione checkboxes de consentimento
e deixe clara a finalidade do uso dos dados (piloto do EcoBag+).

Boa validação! 🌱
