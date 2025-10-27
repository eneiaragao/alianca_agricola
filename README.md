# 🚜 Landing Page: Manutenção e Peças New Holland (Formosa e Região)

Este projeto é uma Landing Page de alta conversão, desenvolvida em HTML, CSS e JavaScript puro, otimizada especificamente para campanhas de **Tráfego Pago** (Google Ads, Meta/Facebook Ads). O objetivo principal é capturar leads para serviços de manutenção, serviços de campo e venda de peças para máquinas agrícolas New Holland na região de Formosa/GO.

## 🎯 Objetivo Principal

**Capturar o contato (WhatsApp ou Formulário) do produtor rural em situação de urgência (máquina parada).**

## ✨ Funcionalidades e Foco em Conversão

| Recurso | Descrição | Status |
| :--- | :--- | :--- |
| **Arquitetura CTA** | Múltiplos Call-to-Actions (CTAs) em locais estratégicos (topo, hero e rodapé). | Implementado |
| **Atendimento WhatsApp** | Links `wa.me` diretos com mensagem pré-preenchida, usando o número **(61) 99632-7726**. | Implementado |
| **Captura de Leads** | Formulário de contato simples (Nome e WhatsApp) para minimizar o atrito. | Implementado |
| **Backend Simplificado** | Integração via **FormSubmit** para receber leads por e-mail em **`eneiaragao@gmail.com`**. | Implementado |
| **Foco Geográfico** | Títulos e textos mencionam Formosa e Região para maior relevância nas campanhas. | Implementado |

## ⚙️ Configuração e Integração

Para colocar a Landing Page no ar e garantir que a captura de leads funcione corretamente, siga estes passos:

### 1. Configuração dos Arquivos

1.  **Arquivo HTML:** O código principal está em um único arquivo, geralmente nomeado `index.html`.
2.  **Arquivos de Mídia:** Crie os arquivos a seguir e garanta que estejam na mesma pasta (ou atualize os caminhos no CSS):
    * **Imagem do Hero:** Substitua o caminho da imagem de fundo no CSS (`background: url('caminho/para/imagem-trator.jpg')`) por uma imagem real de alta qualidade.
    * **Favicon:** Adicione um arquivo `favicon.ico` ou `favicon.png` na raiz do projeto.

### 2. Ativação do FormSubmit (E-mail)

O formulário está configurado para enviar os dados para `eneiaragao@gmail.com` via FormSubmit.

> ⚠️ **Passo Crítico:** Para ativar o recebimento de leads, você deve enviar um formulário de teste e **clicar no link de confirmação** que o FormSubmit envia para `eneiaragao@gmail.com`. Se não fizer isso, os leads não serão entregues.

### 3. Configuração de Rastreamento (Para Anúncios)

Para que as campanhas de tráfego pago sejam otimizadas, o rastreamento de conversão é fundamental.

1.  **Instale os Códigos Base:** Insira o código base do Google Analytics (GA4), Google Ads (Global Site Tag) e/ou Meta/Facebook Pixel dentro da tag `<head>` do `index.html`.
2.  **Rastreie Conversões de Formulário:** Como a página redireciona após o envio do formulário (configuração `_next`), você deve instalar o evento de conversão na **página de sucesso** definida na tag `_next`.

    ```html
    <script>
        // Exemplo Google Ads: 
        // gtag('event', 'conversion', {'send_to': 'AW-XXXXXXXXX/YYYYYYYYY'}); 
    </script>
    ```

3.  **Rastreie Cliques no WhatsApp:** Para maior precisão, configure eventos de clique em todos os links `wa.me` usando as ferramentas de rastreamento (GA4, Meta Pixel etc.).

## 📞 Detalhes de Contato

Os seguintes detalhes foram implementados no código:

* **Telefone de Contato (Ligação):** `(61) 99632-7726`
* **Link WhatsApp:** `https://wa.me/5561996327726`
* **E-mail para Leads (FormSubmit):** `eneiaragao@gmail.com`

---

Desenvolvido por: **[Seu Nome/Nome da Empresa]** *Data de Criação/Última Modificação: Outubro de 2025*
