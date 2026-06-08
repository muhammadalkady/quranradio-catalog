# quranradio-catalog

Public CDN mirror of the **QuranRadio** app's catalog manifest.

`catalog.json` is generated from the public [mp3quran v3 API](https://mp3quran.net/api),
normalized and HEAD-validated, by the app's private build pipeline and pushed here daily.
The app fetches it (with `ETag`/conditional GET) via jsDelivr:

```
https://cdn.jsdelivr.net/gh/muhammadalkady/quranradio-catalog@main/catalog.json
```

This repo holds **only** the generated manifest — it contains no app source.
