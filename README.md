# Telugu-tense-template
A site that helps in identifying the exact tense of a root verb
# Telugu Verb Conjugator — క్రియా రూపాలు

A clean, single-page web app for learning Telugu verb conjugations across all tenses. Built for language learners who struggle with grammatical context changes in Telugu verbs.

## Features

- **25+ common Telugu verbs** with full conjugation tables
- **6 tenses**: Present, Past, Future, Present Continuous, Past Perfect, Imperative
- **7 pronouns** for each tense (నేను, నువ్వు, అతను, ఆమె, మీరు, మేము, వాళ్ళు)
- **Search** by Telugu script, transliteration, or English meaning
- **Category filters**: Common, Motion, Communication, Daily, Emotion
- **Toggle transliteration** on/off for both Telugu script and romanized text
- Fully responsive — works on desktop, tablet, and mobile
- Zero dependencies — pure HTML, CSS, and JavaScript

## Hosting on GitHub Pages

1. Create a new repository on GitHub
2. Upload `index.html` to the repository root
3. Go to **Settings → Pages**
4. Under **Source**, select `main` branch and `/ (root)` folder
5. Click **Save** — your site will be live at `https://<username>.github.io/<repo-name>/`

## Adding More Verbs

Open `index.html` and add entries to the `VERBS` array following this structure:

```javascript
{
  root_te: 'తిను',          // Telugu script root
  root_ro: 'tinu',          // Romanized root  
  meaning: 'to eat',        // English meaning
  category: 'Daily',        // One of: Common, Motion, Communication, Daily, Emotion
  tenses: {
    'Present': [
      ['తింటాను','tiṇṭānu'],   // నేను (I)
      ['తింటావు','tiṇṭāvu'],   // నువ్వు (you inf.)
      ['తింటాడు','tiṇṭāḍu'],   // అతను (he)
      ['తింటుంది','tiṇṭundi'],  // ఆమె (she)
      ['తింటారు','tiṇṭāru'],   // మీరు (you for.)
      ['తింటాము','tiṇṭāmu'],   // మేము (we)
      ['తింటారు','tiṇṭāru']    // వాళ్ళు (they)
    ],
    // ... other tenses
  }
}
```

## License

MIT — free to use and modify.
