# Frutas Falantes IA — Site de Vendas

Site completo e responsivo para vender o kit digital **Frutas Falantes IA — Kit de Criação de Vídeos** por R$ 34,99.

## Arquivos

| Arquivo         | Função                                                        |
|-----------------|---------------------------------------------------------------|
| `index.html`    | Página completa (HTML + CSS + JS embutidos).                  |
| `config.js`     | Configuração do link de checkout da Kiwify.                   |
| `README.md`     | Este guia.                                                    |

> Todas as ilustrações dos personagens são **arte vetorial original** (SVG) criada
> exclusivamente para este projeto — nenhuma imagem de terceiros é usada, então
> não há problemas de licença. Você pode substituí-las depois por imagens geradas
> por IA, se quiser.

## 1. Como publicar de graça (3 opções)

### Opção A — Netlify Drop (mais rápido, ~1 minuto)
1. Acesse https://app.netlify.com/drop
2. Arraste a pasta do projeto para a página.
3. Pronto — o Netlify gera um endereço público tipo `https://seu-site.netlify.app`.

### Opção B — Vercel
1. Acesse https://vercel.com e faça login (grátis).
2. Clique em **Add New → Project → Upload** e envie a pasta.
3. O endereço público será algo como `https://seu-site.vercel.app`.

### Opção C — GitHub Pages
1. Crie um repositório no GitHub e envie os arquivos.
2. Vá em **Settings → Pages → Source: main branch / root**.
3. O site fica disponível em `https://seuusuario.github.io/nome-do-repo`.

## 2. Como ativar o botão de compra (Kiwify)

1. Crie o checkout do produto na **Kiwify** e copie o link público.
2. Abra `config.js` e cole o link:

```js
var CONFIG = {
  checkoutUrl: "https://pay.kiwify.com.br/SEU-CODIGO-AQUI"
};
```

3. Suba o arquivo atualizado para a hospedagem.

Enquanto o campo estiver vazio, o botão exibe um aviso de "configuração pendente"
(nenhum link de pagamento falso é usado).

## 3. Personalizações rápidas

- **Preço:** pesquise por `34,99` no `index.html` e ajuste.
- **Cores:** edite as variáveis no bloco `:root` do CSS (topo do `<style>`).
- **Textos/FAQ:** todas as seções estão comentadas em português no HTML.

## 4. Boas práticas já incluídas

- Layout responsivo (celular, tablet e desktop).
- Navegação suave com âncoras e menu mobile.
- FAQ em acordeão acessível (atributos ARIA).
- Animações com `prefers-reduced-motion` respeitado.
- Sem links quebrados e sem afirmações inventadas (depoimentos, garantias, estatísticas).
- Nota de transparência sobre o kit estar em produção.
