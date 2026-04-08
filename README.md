# J3F Brand Kit 2026

Brand kit oficial da **J3F Consultoria Tributária** — Tax Intelligence.
Fonte canônica pública de logos, tokens de design, tipografia, templates e guia de voz.

![Verde Escuro](https://img.shields.io/badge/verde_escuro-%23005263?style=flat-square) ![Teal](https://img.shields.io/badge/teal-%2300ACCA?style=flat-square) ![Verde Claro](https://img.shields.io/badge/verde_claro-%2396C9D7?style=flat-square) ![Cobre](https://img.shields.io/badge/cobre-%239E947E?style=flat-square)

---

## Estrutura

```
00_Manual/            Síntese do manual de marca (brand-summary.md)
01_Brand_Tokens/      Tokens em JSON, CSS, SCSS, Python, TypeScript
02_Logos/             Logos em PNG, SVG, PDF (RGB e CMYK)
03_Fonts/             Família Manrope (OFL — Open Font License)
04_Templates/         Word, Excel, PowerPoint, Email
05_Assets_Graficos/   Grafismos auxiliares (reservado)
06_Fotografia/        Diretrizes fotográficas (reservado)
07_Writing_Guide/     Guia de tom de voz, vocabulário on/off, taglines
```

---

## Uso — URLs públicas via jsDelivr

Todos os assets são consumíveis via CDN global (jsDelivr, cache de borda):

```
https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/<caminho>
```

**Exemplos:**

| Asset | URL |
|---|---|
| Isotipo verde (PNG) | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/02_Logos/RGB_PNG/J3F_isotipo_verde.png` |
| Isotipo verde (SVG) | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/02_Logos/RGB_SVG/J3F_isotipo_verde.svg` |
| Logo primário verde | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/02_Logos/RGB_PNG/J3F_logo_primario_verde.png` |
| Logo primário branco (fundo verde escuro) | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/02_Logos/RGB_PNG/J3F_logo_primario_branco_fundo_verde_escuro.png` |
| Tokens (JSON) | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/01_Brand_Tokens/brand.json` |
| Tokens (CSS) | `https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/01_Brand_Tokens/brand.css` |

Para travar uma versão, substituir `@main` por uma tag como `@v1.0.0`.

---

## Integração nos apps J3F

### JavaScript / TypeScript

```ts
const brand = await fetch(
  'https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/01_Brand_Tokens/brand.json'
).then(r => r.json());

console.log(brand.colors.primary.verdeEscuro); // "#005263"
```

### Python

```python
import json, urllib.request
url = 'https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/01_Brand_Tokens/brand.json'
brand = json.loads(urllib.request.urlopen(url).read())
verde_escuro = brand['colors']['primary']['verdeEscuro']
```

### HTML / CSS

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/J3F-Tax-Intelligence/brand@main/01_Brand_Tokens/brand.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&display=swap">
```

---

## Paleta oficial

| Cor | Hex | Uso |
|---|---|---|
| **Verde Escuro** | `#005263` | Cor primária, fundos escuros, CTAs |
| **Teal** | `#00ACCA` | Destaque, links, acentos |
| **Verde Claro** | `#96C9D7` | Secundária, backgrounds leves |
| **Cobre** | `#9E947E` | Detalhes, taglines, elementos decorativos |
| **Bege Claro** | `#EEE7D7` | Backgrounds neutros, divisores |
| **Cinza** | `#999999` | Texto secundário |
| Preto | `#000000` | Texto principal |
| Branco | `#FFFFFF` | Fundos claros |

Paleta legacy **descontinuada** (não usar): `#505459`, `#54BFC3`, `#2C3E50`, `#D4A853`.

## Tipografia

**Manrope** (única família oficial). Hospedada localmente em `03_Fonts/` e disponível no Google Fonts.

```
Display     72pt / ExtraBold
H1          48pt / Bold
H2          32pt / SemiBold
H3          24pt / SemiBold
Body large  18pt / Regular
Body        14pt / Regular
Small       12pt / Medium
Caption      9pt / Medium
```

Fontes legacy **descontinuadas**: Georgia, Calibri, Playfair Display, DM Sans.

## Regras de uso dos logos

- **Nunca recriar.** Usar apenas os arquivos originais de `02_Logos/`.
- **Posições permitidas:** superior esquerdo, inferior esquerdo, centralizado.
- **Nunca à direita.**
- **Área de não-interferência:** 1× a altura do logo em todas as direções.
- **Fundos:** variante `branco` sobre fundos escuros; `verde` ou `preto` sobre fundos claros.

Detalhes em [`00_Manual/brand-summary.md`](./00_Manual/brand-summary.md).

## Tom de voz

Pilares: **autoritário acessível**, **vanguardista tech**, **preciso seguro**.

Vocabulário on/off, manifesto, taglines e checklist em [`07_Writing_Guide/tom_voz.md`](./07_Writing_Guide/tom_voz.md).

---

## Taglines

> **Pagando o justo. Nem um centavo a mais.**
> **Precisão técnica. Inteligência fiscal.**
> **Tax Intelligence.**

---

## Licença

[CC BY-NC-ND 4.0](./LICENSE). Uso permitido em contextos relacionados à J3F Consultoria Tributária. Reprodução dos logos sujeita às regras do manual de marca.

Contato: **fabio@j3f.com.br**
