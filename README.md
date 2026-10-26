# English-sef

A single-page Sefaria reader that shows Hebrew beside English for everything. Where Sefaria has a translation you get Sefaria's; where it has none (most commentaries, midrash and halakhah), the reader fills in a labelled machine translation.

Live: https://gideonpotok.github.io/English-sef/

- Home shows today's learning calendar (parasha, haftarah, Daf Yomi, Daily Mishnah, Rambam…).
- Search resolves references and names in Hebrew or English through Sefaria's name API.
- Tap a segment for its connections, grouped by category; each commentator is tagged EN (Sefaria has English) or MT (machine translation).
- Nikud toggle, Both / English / Hebrew views, prev/next navigation.
- No build, no dependencies: `index.html` is the whole app.

Texts come from the [Sefaria API](https://developers.sefaria.org/) under their respective licenses. Machine translation uses Google Translate's public, keyless endpoint; if it is unreachable the Hebrew still shows.
