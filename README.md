# Adguard_filter
### StevenBlack-hosts-Pornblock
umgeformt von https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/porn/hosts
### Weitere Websites wurden von _PornDude_ gescraped

# Angewandte Befehle in VS22 zum umformen der _StevenBlack-hosts-Pornblock_ list:
- Win+H
- .* An (Regex - sonst wird nichts gefunden)
- Suchen: \|\|\s*([A-Za-z0-9\.-]+)(?:\s*-\s*([A-Za-z0-9\.-]+))*
- Ersetzen Durch: ||$0^$category=adult

# PornDude 
- In jedes Fenster rein gehen Website öffnen und schauen ob die Seite erreichbar ist - Wenn ja, wird Sie in die liste hinzugefügt
- Mit Ki Umformen
- VSStudio 22 öffnen
- .* Anwählen (Regex - sonst wird nichts gefunden)
### URLs in Domains umformen
- Suchen: https?://(?:www\.)?([^/?#]+)[^ \r\n]*
- Ersetzen: ||$1^$category=adult
### Duplikate entfernen
- Strg + A (Alles Markieren)
- Shift + Alt + L (Danach)
- Shift + Alt + S (Sortiert die liste)
- Suchen: ^(.*)(\r?\n\1)+$
- Ersetzen: <Leer lassen>
- Strg + A (Alles Markieren)
- Shift + Alt + L (+ Danach)
- Shift + Alt + S (Sortiert die liste)
