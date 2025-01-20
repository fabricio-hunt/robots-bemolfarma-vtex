# Documentação do arquivo robots.txt

Este repositório descreve a configuração do arquivo `robots.txt` utilizado no site da Bemol Farma. Este arquivo é usado para controlar o acesso de robôs e spiders a partes específicas do site, assegurando o desempenho e a privacidade de determinadas áreas.

---

## Estrutura do `robots.txt`

### Regras Gerais

As seguintes regras são aplicadas a todos os robôs (User-agents):

```txt
User-agent: *
Allow: /
Disallow: /finalizacao/carrinho
Disallow: /account*
Disallow: /*/?map=productClusterIds
Disallow: /listas*
Disallow: /appnativo*
Disallow: /Custom/Content/Themes/BemolFarma/Templates/landings*
Disallow: /web-api/v1/Shopping/Seller*
Disallow: /Login.partial?Url=/appnativo*
Disallow: /login
Disallow: /lista-teste
Disallow: /pagina-teste*
Disallow: /*map=
```

### Regras Específicas

#### Screaming Frog SEO Spider
- Permissão total:

```txt
User-agent: Screaming Frog SEO Spider
Allow: /
```

#### EtaoSpider
- Bloqueio total:

```txt
User-agent: EtaoSpider
Disallow: /
```

#### GPTBot
- Bloqueio total:

```txt
User-agent: GPTBot
Disallow: /
```

#### CCBot
- Bloqueio total:

```txt
User-agent: CCBot
Disallow: /
```

---

## Sitemap

O arquivo `robots.txt` também inclui uma referência ao sitemap do site, que está localizado em:

```txt
Sitemap: https://www.bemolfarma.com.br/sitemap.xml
```

---

## Como funciona o `robots.txt`

1. **User-agent**: Especifica qual robô ou spider será afetado pelas regras subsequentes.
2. **Allow**: Permite o acesso a uma URL ou padrão de URL.
3. **Disallow**: Bloqueia o acesso a uma URL ou padrão de URL.
4. **Sitemap**: Fornece o caminho do sitemap do site para facilitar a indexação por motores de busca.

---

## Propósito das Regras

- **Desempenho**: Evitar que robôs sobrecarreguem o servidor acessando URLs irrelevantes ou sensíveis.
- **Segurança**: Proteger informações e áreas privadas do site.
- **SEO**: Direcionar os robôs para as áreas mais relevantes, garantindo que as páginas importantes sejam indexadas corretamente.

---

## Contribuições

Se você deseja sugerir melhorias ou relatar problemas relacionados ao arquivo `robots.txt`, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

---

## Referências

- [Documentação oficial do robots.txt](https://developers.google.com/search/docs/crawling-indexing/robots-txt?hl=pt-br)
- [Validador de robots.txt](https://www.google.com/webmasters/tools/robots-testing-tool)

---

**Autor:** Bemol Farma

**Contato:** [suporte@bemolfarma.com.br](mailto:suporte@bemolfarma.com.br)

