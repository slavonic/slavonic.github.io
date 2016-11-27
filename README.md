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
   
   Your valuable thoughts
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
   
   Ваши умные мысли
   ```
3. Again, note that you are not restricted to the `default` layout template. But you better use the same layout
   as in English version of this page
4. Note that `ref` value must be exactly the same as in the English page
5. 
