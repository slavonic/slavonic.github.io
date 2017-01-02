# slavonic.github.io

Source of `sci.ponomar.net` website. 

You can check live version of this site at https://slavonic.github.io

## How to add a page

1. create a new Markdown or HTML page. Give the file a descriptive name. For example, `thoughts.md`
2. add YAML header like this:
   ```
   ---
   layout: default
   ref: thoughts
   lang: en
   ---
   
   My valuable thoughts
   ```
3. Note that you can yse any valid layout template for this new file, not necessarily a `default` one
4. Note that you must supply a unique `ref` value. Best convention is to use the file name without extension
5. Note that you must specify `lang`. Always create `lang: en` page first, because `en` is the default language of this
   site

Now, lets add a translation to `ru`

1. create a file in `/ru/` directory named `thoughts.md`
2. add YAML header like this:
   ```
   ---
   layout: default
   ref: thoughts
   lang: ru
   ---
   
   Мои умные мысли
   ```
3. Again, note that you are not restricted to the `default` layout template. But you better use the same layout
   as in English version of this page
4. Note that `ref` value must be exactly the same as in the English page
5. Note that lang is declared to be `ru`

## Conventions

1. Place translations under top-level directory with the language name
2. Mirror website tree in each language directory
3. Use `ref` as file name base. Name of translated page file is the same as the name of the English file. 
   The only difference is that translated page resides under its language directory tree

## Navigational and other site-wide information

Information global to the site (title, authors, keywords) is stored in `_config.yaml`. It is used in templates and content
by utilizing Liquid templating language. For example, `authors` data from `_config.yaml` is used in `legal.md` like this:

```
{{ site.authors[page.lang] }}
```

Note that navigational and global information has to be provided for all supported languages (unlike content pages
that may skip a language if needed). This is because this information may be used from any page and is often used by
templates (meaning that every page embeds this data).

Information that is specific to the site navigation bar is in `_data/nav.yaml`.

Footer data is specified in `_data/footer_left.yaml` and `_data/footer_right.yaml`.
