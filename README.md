# English-sef

A single-page Sefaria reader that shows Hebrew beside English for everything. Where Sefaria has a translation you get Sefaria's; where it has none (most commentaries, midrash and halakhah), the reader fills in a labelled machine translation.

Live: https://gideonpotok.github.io/English-sef/

- Home shows today's learning calendar (parasha, haftarah, Daf Yomi, Daily Mishnah, Rambam…).
- Search resolves references and names in Hebrew or English through Sefaria's name API.
- Tap a segment for its connections, grouped by category; each commentator is tagged EN (Sefaria has English) or MT (machine translation).
- Nikud toggle, Both / English / Hebrew views, prev/next navigation.
- No build, no dependencies: `index.html` is the whole app.

Texts come from the [Sefaria API](https://developers.sefaria.org/) under their respective licenses. Machine translation runs through a chain of providers: Google's free endpoint, Google's dictionary endpoint, then MyMemory; a provider that fails or rate-limits is rested and the next one takes over. Under **Translators** you can add a Claude API key (noticeably better on rabbinic Hebrew; can be set to go first) or a Google Cloud Translation key. Keys stay in the browser's localStorage.
