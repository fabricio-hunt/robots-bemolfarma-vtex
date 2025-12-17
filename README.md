

# robots.txt File Documentation

This repository describes the configuration of the `robots.txt` file used on the Bemol Farma website. This file is used to control access by robots and spiders to specific parts of the site, ensuring performance and privacy for certain areas.

---

## `robots.txt` Structure

### General Rules

The following rules apply to all robots (user-agents):

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

### Specific Rules

#### Screaming Frog SEO Spider

* Full access allowed:

```txt
User-agent: Screaming Frog SEO Spider
Allow: /
```

#### EtaoSpider

* Fully blocked:

```txt
User-agent: EtaoSpider
Disallow: /
```

#### GPTBot

* Fully blocked:

```txt
User-agent: GPTBot
Disallow: /
```

#### CCBot

* Fully blocked:

```txt
User-agent: CCBot
Disallow: /
```

---

## Sitemap

The `robots.txt` file also includes a reference to the site’s sitemap, located at:

```txt
Sitemap: https://www.bemolfarma.com.br/sitemap.xml
```

---

## How `robots.txt` Works

1. **User-agent**: Specifies which robot or spider the following rules apply to.
2. **Allow**: Permits access to a URL or URL pattern.
3. **Disallow**: Blocks access to a URL or URL pattern.
4. **Sitemap**: Provides the location of the site’s sitemap to facilitate indexing by search engines.

---

## Purpose of the Rules

* **Performance**: Prevent robots from overloading the server by accessing irrelevant or sensitive URLs.
* **Security**: Protect private information and restricted areas of the site.
* **SEO**: Guide robots to the most relevant areas, ensuring important pages are indexed correctly.

---

## Contributions

If you would like to suggest improvements or report issues related to the `robots.txt` file, feel free to open an *issue* or submit a *pull request*.

---

## References

* [Official robots.txt documentation](https://developers.google.com/search/docs/crawling-indexing/robots-txt)
* [robots.txt Validator](https://www.google.com/webmasters/tools/robots-testing-tool)

---

**Author:** Bemol Farma


---
