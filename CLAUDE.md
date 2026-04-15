# CLAUDE.md — CALEOPRECONCEITO

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** CALEOPRECONCEITO
**Nicho:** Esportes e Fitness
**Keywords:** Conheca um pouco do nosso Corinthians Bem vindos ao site oficial do
**Paleta de cores:** rose | **Fonte:** montserrat

Conheça um pouco do nosso Corinthians Bem-vindos ao site oficial do Futebol Feminino do Corinthians! Nós somos uma equipe apaixonada pelo esporte e determinada a mudar o cenário do futebol feminino no Brasil. Acreditamos que o esporte deve ser para todos, independentemente de gênero, e estamos comprometidos em acabar com o preconceito e atrair mais público para o futebol feminino. A história do Futebol Feminino do Corinthians é marcada por grandes conquistas e por uma trajetória de luta pela igualdade de gênero no esporte. Desde a sua fundação, em 2016, a equipe vem quebrando barreiras e desafiando estereótipos, sempre com muita garra e determinação. Nós acreditamos que o futebol feminino tem o poder de transformar a sociedade, promovendo a inclusão, a diversidade e o respeito. Queremos inspirar outras pessoas a se juntarem a nós nessa luta, construindo um futuro mais justo e igualitário para o esporte. Nosso objetivo é criar uma experiência única para os nossos torcedores, oferecendo um futebol de qualidade e uma atmosfera acolhedora em nossos jogos. Queremos que todos se sintam bem-vindos em nossos estádios, independentemente do gênero, idade ou origem. Por isso, pedimos o apoio de todos os nossos fãs e seguidores para que possamos levar o Futebol Feminino do Corinthians a novos patamares. Juntos, podemos construir um futuro melhor para o esporte, baseado na igualdade, na inclusão e no respeito. Obrigado por visitar o nosso site e se juntar a nós nessa jornada!



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-G |
| Features | Features-J |
| About Section | About-G |
| Posts | Posts-H |
| Footer | Footer-A |
| Página Sobre | Sobre-E |
| Página Contato | Contato-B |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
