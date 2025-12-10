# Tehniskās piezīmes (TECH NOTES)

## Izmantotās tehnoloģijas
- HTML — lietotnes struktūra
- JavaScript — datu ielāde no Supabase
- Supabase — datubāze un API
- GitHub Pages — publiskais hostings
- GitHub — versiju kontrole un PR

## Konfigurācijas faili
- `index.html` satur JavaScript kodu ar Supabase savienojumu
- `.env.example` var saturēt fiktīvas atslēgas
- Privātās atslēgas **repā nedrīkst likt**

## Supabase savienojums
`index.html` failā ir rinda:

```js
const { data, error } = await supabase
  .from("members")
  .select("*");
