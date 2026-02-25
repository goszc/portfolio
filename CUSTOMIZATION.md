# Guia Rápido de Customização

Referência para personalizar este template para cada cliente.

---

## 1. Trocar Cores (3 variáveis)

Abra `style.css` e edite o bloco `:root` no topo:

```css
:root {
  --color-primary: #2563EB;       /* Cor principal da marca */
  --color-primary-dark: #1D4ED8;  /* Tom mais escuro (hover) */
  --color-primary-light: #60A5FA; /* Tom claro */
  --color-primary-ultra-light: #DBEAFE; /* Fundo sutil */
  --color-accent: #F97316;        /* Cor do botão CTA */
  --color-accent-hover: #EA580C;  /* CTA hover */
}
```

**Dica:** Use [coolors.co](https://coolors.co) para gerar paletas. Troque `--color-primary` e `--color-accent`, e derive as variantes (dark, light, ultra-light) a partir delas.

---

## 2. Trocar Fontes

No `:root` do `style.css`:
```css
--font-heading: 'Poppins', sans-serif;
--font-body: 'Open Sans', sans-serif;
```

E no `<head>` do `index.html`, atualize o link do Google Fonts:
```html
<link href="https://fonts.googleapis.com/css2?family=NOVA+FONTE..." rel="stylesheet">
```

---

## 3. Adicionar/Remover Seções

Cada seção está marcada com comentários no HTML:
```html
<!-- SECTION: Galeria -->
<section class="gallery section" id="galeria">
  ...
</section>
```

- **Remover:** Delete o `<section>` inteiro e o link correspondente no menu.
- **Adicionar:** Copie uma seção existente e adapte.

---

## 4. WhatsApp

No `index.html`, troque o número em TODOS os links WhatsApp:
```
https://wa.me/55SEU_NUMERO?text=Mensagem
```

Formato: `55` + DDD + número (sem espaços ou traços).

---

## 5. Google Maps

No `index.html`, seção Contato, troque o `src` do iframe:
1. Abra [Google Maps](https://maps.google.com)
2. Busque o endereço
3. Clique em "Compartilhar" → "Incorporar um mapa"
4. Copie somente a URL do `src`

---

## 6. Serviços

Na seção `#servicos`, cada card segue este padrão:
```html
<div class="service-card reveal">
  <div class="service-card__icon">
    <!-- SVG do ícone -->
  </div>
  <h3 class="service-card__title">Nome</h3>
  <p class="service-card__desc">Descrição</p>
</div>
```

Ícones SVG: use [Lucide Icons](https://lucide.dev/icons) — copie o SVG.

---

## 7. Imagens

Substitua os placeholders por `<img>`:
```html
<!-- Antes (placeholder) -->
<div class="hero__image-placeholder">...</div>

<!-- Depois (imagem real) -->
<img src="img/hero.jpg" alt="Descrição da imagem" class="hero__image">
```

---

## 8. Redes Sociais

No footer, troque os `href` dos links:
```html
<a href="https://instagram.com/CLIENTE" ...>
<a href="https://facebook.com/CLIENTE" ...>
```

---

## 9. Informações de Contato

Seção `#contato` → Atualize:
- Endereço
- Telefone
- E-mail

Seção `#agendar` → Atualize:
- Link do WhatsApp
- Número de telefone

Footer → Atualize:
- Nome do negócio
- Ano do copyright
