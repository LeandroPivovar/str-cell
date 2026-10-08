# STRCELL | Conserto de celulares e consoles com delivery

Site institucional da STRCELL (WhatsApp: "Samuel Terra Rodrigues"). HTML/CSS/JS estático, sem build. Mesma
estrutura dos outros sites da AROE, em tema claro com o azul-marinho da logo. O foco é o diferencial do perfil:
**busca e entrega do aparelho** e conserto em até 1 hora quando possível.

```bash
npx --yes serve . -l 6410
```

## Estrutura

```
index.html
assets/
  css/styles.css
  js/main.js              menu mobile, formulário -> WhatsApp, FAQ, reveal ao rolar, ano do rodapé
  fonts/phosphor/         ícones Phosphor (woff2 local, licença MIT)
  img/icon.svg            ícone da logo redesenhado em SVG (celular + chave + engrenagem), também é o favicon
```

Sem fotos: o hero tem um celular "em conserto" e um controle de console feitos em CSS/ícones.

## Dados usados (fonte: perfil do WhatsApp Business)

| Campo | Valor |
|---|---|
| Nome | STRCELL (perfil: "Samuel terra rodrigues") |
| Descrição | Conserto de celulares e consoles, delivery. Busco e entrego. Se possível faço o serviço em 1h. Dependendo do local não cobro taxa de deslocamento. Precisou pode chamar. |
| WhatsApp | (48) 99639-4912 (`wa.me/554896394912`, constante `WA` no `main.js`) |
| Horário | 09:00 às 22:00 |
| Instagram | o perfil traz `https://www.instagran/strcell` (com erro de digitação); o site usa `instagram.com/strcell` |

Os textos estão em primeira pessoa ("eu busco e entrego"), como o próprio perfil.

## Confirmar com o cliente

- **Instagram:** confirmar se o @ é mesmo `strcell` (o link do perfil está quebrado: "instagran").
- **Cidade / região de atendimento:** o perfil não diz. O DDD 48 é da Grande Florianópolis, mas o site não cita
  cidade. Saber os bairros/cidades onde não cobra deslocamento ajudaria muito (FAQ e SEO).
- **Lista de defeitos:** celulares (tela, bateria, conector, câmera/som, não liga) e consoles (não liga,
  superaquecimento, sem imagem, limpeza, controles) são os consertos mais comuns. Confirmar o que faz e quais
  consoles atende (PlayStation, Xbox, Nintendo?).
- **Dias de atendimento:** só o horário (9h às 22h) é conhecido.
- **Telefone:** o perfil mostra `9639-4912`. O `wa.me` usa o número do perfil; o texto exibido usa
  `(48) 99639-4912`, com o 9 do celular.
- **Logo:** a logo da capa tem resolução baixa e o texto pequeno ("S... specialized technical assistance") fica
  coberto pela foto. Pedir o arquivo original para trocar o ícone redesenhado.

## Depoimentos

Não foram incluídos, para não publicar avaliações inventadas.

Fontes: Montserrat e Inter (Google Fonts, OFL).

## Deploy

Sem build: publicar a pasta na Vercel, GitHub Pages ou hospedagem comum.
Depois do deploy, adicionar `og:image` (URL absoluta) e `<link rel="canonical">`.
