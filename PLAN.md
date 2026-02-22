# Portfolio Website Plan — Ney Carvalho

Freelance web developer based in Arlon, Belgium.
Target: Portuguese-speaking small businesses in Luxembourg and Portugal.

---

## 1. Stack Recommendation

**Astro + Tailwind CSS, deployed on Vercel.**

| Why Astro over Next.js? | Reason |
|---|---|
| Zero JS by default | Faster load = better SEO, better mobile experience for non-tech clients browsing on phone |
| Simpler for a static portfolio | No auth, no database, no dynamic routes needed |
| Still supports React islands | If Ney wants an interactive contact form or animation, drop in a React component |
| Tailwind works natively | Same styling workflow Ney already knows |
| Deploys to Vercel in 1 click | Same platform as his client projects |

**If Ney strongly prefers Next.js** — use Next.js App Router with static export (`output: 'export'`). It works fine, just ships more JS than needed for a brochure site.

**Form backend:** Formspree (free tier, 50 submissions/month) or Resend for email delivery. No Supabase needed — keep it simple.

---

## 2. Pages & Sections

**Single-page site with anchor navigation.** Reason: the target audience (small business owners) won't click through 5 pages. They scroll. One page, one story, one CTA.

Optional separate page: `/caso/joterapeutacapilar` for a detailed case study (helps SEO).

### Homepage sections (in scroll order):

| # | Section | Purpose |
|---|---|---|
| 1 | **Hero** | Name, tagline, CTA button |
| 2 | **Problem** | "You have a business but no website" — speak to their pain |
| 3 | **Services** | What Ney builds (sites, booking systems, e-commerce) |
| 4 | **Pricing** | Transparent packages with starting prices |
| 5 | **Portfolio / Case Study** | JoTerapeutaCapilar showcase + future projects |
| 6 | **About** | Who is Ney, why trust him |
| 7 | **Process** | How it works in 3-4 simple steps |
| 8 | **FAQ** | Common objections answered |
| 9 | **Contact / CTA** | WhatsApp button + simple form |
| 10 | **Footer** | Links, legal, social |

---

## 3. Design Direction

### Mood
**Professional but warm. Modern but not intimidating.**

The audience is a 40-year-old Portuguese restaurant owner in Luxembourg who has never hired a developer. The site must feel like talking to a helpful neighbor, not a tech company.

### Colors

| Role | Color | Hex | Why |
|---|---|---|---|
| Primary | Deep teal/petrol blue | `#0F4C5C` | Professional, trustworthy, not corporate |
| Accent | Warm gold/amber | `#E8A838` | Warmth, energy, stands out on dark backgrounds |
| Background | Off-white | `#FAFAF7` | Clean, easy on the eyes |
| Text | Near-black | `#1A1A2E` | Readable |
| Secondary bg | Light warm gray | `#F0EDE8` | For alternating sections |

Avoid: red/green (Portuguese flag cliche), pure black backgrounds, neon colors.

### Typography

| Use | Font | Why |
|---|---|---|
| Headings | **Inter** or **DM Sans** | Clean, modern, highly readable |
| Body | **Inter** | Same family, consistent, excellent at small sizes |
| Accent (optional) | **Playfair Display** | For the hero tagline only — adds personality |

Keep it to 2 fonts max. Load from Google Fonts or self-host for performance.

### Style principles
- Generous whitespace — don't crowd
- Rounded corners on cards and buttons (friendly, not sharp)
- Subtle shadows, no heavy borders
- Real screenshots over abstract illustrations
- Mobile-first — most clients will see this on their phone via WhatsApp link

---

## 4. Key Content

### Language Strategy

**⚠️ CRÍTICO: Português de Portugal (PT-PT) — sem excepções.**

Regras obrigatórias:
- "telemóvel" (não "celular"), "frigorífico" (não "geladeira")
- "o seu negócio" (nunca "seu negócio" sem artigo)
- "a seguir", "a partir de", "poupar" (não "economizar")
- Evitar qualquer expressão tipicamente brasileira
- Tom: directo, próximo, profissional. Nem demasiado formal, nem informal.

**Língua única: PT-PT.** A audiência são portugueses da diáspora — reconhecem PT-BR imediatamente e quebra a confiança.

Fase 2 (se necessário): adicionar versão `/fr` para clientes luxemburgueses nativos.

### Hero Section

**Headline:**
> O seu negócio merece um site profissional.

**Subheadline:**
> Crio websites modernos e acessíveis para negócios portugueses no Luxemburgo e em Portugal. Sites que trazem clientes.

**CTA Button:**
> Fala comigo no WhatsApp

### Problem Section

**Headline:** Porque é que precisa de um site?

Content points (short paragraphs or icon cards):
- "Os seus clientes pesquisam no Google antes de visitar"
- "Um site profissional transmite confiança"
- "Marcações online poupam tempo — seu e dos seus clientes"
- "Os seus concorrentes já têm site"

### Services Section

**Headline:** O que eu construo

Three cards:

| Service | Description | Starting at |
|---|---|---|
| Site Profissional | Site de 5 paginas com design moderno, otimizado para telemovel e Google. Perfeito para restaurantes, saloes, clinicas. | a partir de €600 |
| Loja Online | Venda os seus produtos online com pagamento seguro e gestao de stock. | a partir de €1.000 |
| Sistema de Marcacoes | Os seus clientes marcam online, o senhor/a senhora gere tudo num painel simples. Sem papel, sem confusao. | sob consulta |

### Pricing Section

**Show prices. Absolutely.** Reasons:
- Target clients are price-sensitive small business owners
- Hidden prices feel sketchy to non-tech people
- Showing prices filters out bad-fit leads — saves time
- €600 is very competitive — it's an advantage, not a weakness

**Format:** Simple package cards (not a complex comparison table).

| Package | What's included | Price |
|---|---|---|
| **Essencial** | Site de 5 paginas, design responsivo, formulario de contacto, otimizacao basica para Google, 1 mes de suporte | €600 |
| **Comercio** | Tudo do Essencial + loja online, pagamento seguro, gestao de produtos, painel de administracao | €1.000 |
| **Personalizado** | Sistemas de marcacao, paineis de gestao, funcionalidades sob medida | Sob consulta |

Add below the cards:
> "Todos os sites incluem: hospedagem no primeiro ano, certificado SSL, design adaptado ao telemovel, e entrega em 2-4 semanas."

### About Section

**Headline:** Quem sou eu

Key points to include:
- Name: Ney Carvalho
- Based in Arlon, Belgium (close to Luxembourg — mention this)
- Portuguese-speaking — "Trabalhamos na nossa língua"
- Tech stack mention (briefly, non-technical): "Utilizo as mesmas tecnologias que empresas como Netflix e Twitch"
- Why he does this: "Ajudo negócios da nossa comunidade a ter presença online profissional"
- Photo of Ney (important for trust — people hire people, not logos)

### Process Section

**Headline:** Como funciona

4 steps with icons:

1. **Conversa** — "Falamos sobre o seu negócio e o que necessita" (WhatsApp/call)
2. **Proposta** — "Envio um orçamento claro, sem surpresas"
3. **Construcao** — "Crio o seu site em 2-4 semanas com actualizações regulares"
4. **Lancamento** — "O seu site fica online e começa a atrair clientes"

### FAQ Section

Questions to answer:
- "Preciso de saber algo tecnico?" — Não, eu trato de tudo.
- "Quanto tempo demora?" — 2-4 semanas dependendo do projeto.
- "E se eu quiser mudar alguma coisa depois?" — Ofereço 1 mês de suporte incluído. Alterações adicionais são combinadas.
- "Posso ver exemplos do seu trabalho?" — Sim! Veja o caso da Josianne abaixo.
- "Como funciona o pagamento?" — 50% no início, 50% na entrega.

---

## 5. Portfolio / Case Study Section

### On the homepage

A highlight card with:
- Screenshot of JoTerapeutaCapilar.com (desktop + mobile mockup)
- Client name: "Josianne Gomes — Terapeuta Capilar"
- One-line result: "Site profissional com sistema de marcações e blog, em 3 línguas"
- Link to full case study

### Detailed case study page (`/caso/joterapeutacapilar`)

Structure:
1. **Client context** — Who is Josianne, what she does, where she's based
2. **The challenge** — Needed a professional online presence with booking, multilingual support, blog
3. **The solution** — What Ney built (list features: booking system, client portal, blog, multilingual, gallery)
4. **Screenshots** — 3-4 key screens (hero, booking flow, mobile view, admin panel if allowed)
5. **Results** — Any metrics? "X marcações no primeiro mes" — even anecdotal results work
6. **Tech used** — Next.js, Supabase, Tailwind (brief, for credibility)
7. **Client quote** — Get a testimonial from Josianne if possible

### Mockup strategy for future projects

Until Ney has more real clients:
- Create 2-3 **concept mockups** for typical target businesses:
  - A Portuguese restaurant in Luxembourg
  - A hair salon / barbershop
  - A small clinic or therapy practice
- Use Figma or build real demo pages
- Label them clearly as "Conceito" (concept) — don't fake real clients
- These show potential clients "this could be YOUR site"

---

## 6. Contact Strategy

### Primary: WhatsApp button (floating + in CTA sections)

Why WhatsApp:
- Portuguese community in Luxembourg lives on WhatsApp
- Lower barrier than email for non-tech people
- Immediate, personal, familiar
- Use `https://wa.me/XXXXXXXXXXX?text=Ola%20Ney%2C%20vi%20o%20seu%20site%20e%20gostaria%20de%20saber%20mais` (pre-filled message)

### Secondary: Simple contact form

Fields: Nome, Email, Mensagem. That's it. No phone number field, no dropdown menus, no captcha visible to user.

Backend: Formspree or Resend — sends to Ney's email.

### Optional: Phone number displayed

If Ney is comfortable, show a phone number in the footer. Some older clients prefer calling.

### Do NOT include:
- Calendly or booking widgets (overkill for a portfolio)
- Live chat (Ney can't monitor it)
- Social media links unless he has active business profiles

---

## 7. Domain & Hosting

### Hosting: Vercel (free tier)

- Ney already deploys client sites there
- Free SSL, global CDN, automatic deploys from Git
- More than enough for a portfolio site
- Custom domain support included

### Domain name ideas

Priority: short, professional, easy to say on the phone.

| Option | Available? | Notes |
|---|---|---|
| `neydev.pt` | Check | Short, memorable, .pt signals Portuguese market |
| `neycarvalho.com` | Check | Personal brand, professional |
| `neycarvalho.dev` | Check | Modern, developer-oriented |
| `neysites.com` | Check | Action-oriented, easy to remember |
| `sitesparavocê.com` | Check | Benefit-focused, Portuguese |
| `neydigital.com` | Check | Clean, professional |

**Recommendation:** `neycarvalho.com` or `neydev.pt` — personal brand + memorable.

**Registrar:** Namecheap or Porkbun (cheapest .com/.dev). For .pt domains, use dns.pt or a Portuguese registrar.

---

## 8. Timeline Estimate

With AI-assisted development (Claude Code + Cursor/similar):

| Phase | Tasks | Duration |
|---|---|---|
| **Design** | Finalize colors, layout, content in Figma or directly in code | 1 day |
| **Build** | Scaffold Astro project, build all sections, responsive design | 2-3 days |
| **Content** | Write final copy, gather screenshots, create mockups | 1-2 days |
| **Polish** | Animations, SEO meta tags, performance optimization, testing | 1 day |
| **Deploy** | Domain setup, Vercel deploy, final checks | Half day |

**Total: 5-7 days of focused work.**

This assumes Ney provides: his photo, any client testimonials, and final approval on copy.

---

## 9. SEO Basics

### Target keywords

Primary (Portuguese):
- `criação de sites luxemburgo`
- `web developer portugues luxemburgo`
- `criar site para restaurante`
- `site profissional para negócios`
- `fazer site para empresa luxemburgo`

Secondary:
- `site para salao de beleza`
- `loja online para negócios portugueses`
- `web designer arlon belgica`
- `site barato luxemburgo`

### Technical SEO checklist

- [ ] Semantic HTML (`<main>`, `<section>`, `<article>`, `<h1>`-`<h3>` hierarchy)
- [ ] Single `<h1>` per page with primary keyword
- [ ] Meta title: "Ney Carvalho — Criacao de Sites para Negocios Portugueses no Luxemburgo"
- [ ] Meta description: 155 chars, includes CTA and key benefit
- [ ] Open Graph tags for WhatsApp/social sharing previews
- [ ] `alt` text on all images
- [ ] Sitemap.xml
- [ ] robots.txt
- [ ] Page speed: target 95+ Lighthouse score (Astro makes this easy)
- [ ] Mobile-responsive (test on real devices)
- [ ] Schema.org LocalBusiness markup (helps Google show location info)
- [ ] Google Business Profile (free, critical for local searches)

### Content SEO

- Write a blog post or two eventually: "5 razoes para o seu negocio ter um site" — targets long-tail keywords and shows expertise
- Case study page naturally targets "[client industry] + site" keywords

### Local SEO

- Register on Google Business Profile as a web developer in Arlon/Luxembourg area
- Mention "Luxemburgo" and "Portugal" naturally in copy
- Get backlinks from Portuguese community directories in Luxembourg if they exist

---

## 10. Summary of Decisions Needed from Ney

Before building, Ney should confirm:

1. **Stack:** Astro or Next.js?
2. **Domain:** Which domain name? (Check availability first)
3. **Photo:** Does he have a professional headshot?
4. **Testimonial:** Can he get a quote from Josianne?
5. **WhatsApp number:** Which number for the contact button?
6. **Pricing:** Are the €600/€1000 prices final and public?
7. **Language:** PT only, or add FR/EN?
8. **Mockups:** Should we create concept designs for fake businesses?

---

## Next Steps

1. Ney reviews and approves this plan
2. Register domain
3. Scaffold the project
4. Build section by section (Hero -> Problem -> Services -> Pricing -> Portfolio -> About -> Process -> FAQ -> Contact)
5. Deploy to Vercel
6. Set up Google Business Profile
