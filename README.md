# SmartUs Player – AI Translate language packs

Offline translation models used by **SmartUs Player** (Windows) for its AI Translate subtitles.
The app downloads only the packs a chosen language pair needs from the release
[`packs-v1`](https://github.com/SmartUs-ak/smartus-player-models/releases/tag/packs-v1):

    https://github.com/SmartUs-ak/smartus-player-models/releases/download/packs-v1/<pair>.zip

Each zip holds one CTranslate2 model (int8, about 80 MB unpacked): `model.bin`, `config.json`, vocabulary,
`source.spm`, `target.spm` and `ATTRIBUTION.txt`. Pairs without a direct model are translated through English.

## Credit and licence

The models are **OPUS-MT / Tatoeba-MT** by the Language Technology Research Group at the
University of Helsinki (Jörg Tiedemann et al.), licensed under
[CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/). See <https://github.com/Helsinki-NLP/Opus-MT>.

Changes: the original Marian releases were converted to CTranslate2 format with int8 weights by
SmartUs (no retraining). Each pack's `ATTRIBUTION.txt` links its original release.

## Packs (51)

Multi-language models need a target-language token at the start of each input line (last column).

| Pack | Languages | Zip | Target token used |
|---|---|---|---|
| `ar-de` | Arabic → German | 72 MB | – |
| `ar-en` | Arabic → English | 70 MB | – |
| `ar-es` | Arabic → Spanish | 74 MB | – |
| `ar-fr` | Arabic → French | 71 MB | – |
| `ar-it` | Arabic → Italian | 71 MB | – |
| `ar-ru` | Arabic → Russian | 71 MB | – |
| `ar-tr` | Arabic → Turkish | 74 MB | – |
| `bn-en` | Bengali → English | 68 MB | – |
| `de-ar` | German → Arabic | 72 MB | `>>ara<<` |
| `de-en` | German → English | 69 MB | – |
| `de-es` | German → Spanish | 70 MB | – |
| `de-fr` | German → French | 71 MB | – |
| `de-it` | German → Italian | 71 MB | – |
| `en-ar` | English → Arabic | 71 MB | `>>ara<<` |
| `en-de` | English → German | 66 MB | – |
| `en-es` | English → Spanish | 71 MB | – |
| `en-fr` | English → French | 65 MB | – |
| `en-hi` | English → Hindi | 73 MB | – |
| `en-id` | English → Indonesian | 70 MB | – |
| `en-iir` | English → Persian | 67 MB | `>>pes<<` |
| `en-inc` | English → Indic languages | 70 MB | `>>ben<<`, `>>pan_Guru<<` |
| `en-it` | English → Italian | 73 MB | – |
| `en-ru` | English → Russian | 72 MB | – |
| `en-trk` | English → Turkish | 70 MB | `>>tur<<` |
| `en-ur` | English → Urdu | 69 MB | – |
| `en-zh` | English → Chinese | 74 MB | `>>cmn_Hans<<` |
| `es-ar` | Spanish → Arabic | 72 MB | `>>ara<<` |
| `es-de` | Spanish → German | 71 MB | – |
| `es-en` | Spanish → English | 71 MB | – |
| `es-fr` | Spanish → French | 69 MB | – |
| `es-id` | Spanish → Indonesian | 64 MB | – |
| `es-it` | Spanish → Italian | 69 MB | – |
| `es-ru` | Spanish → Russian | 72 MB | – |
| `fr-ar` | French → Arabic | 69 MB | `>>ara<<` |
| `fr-de` | French → German | 69 MB | – |
| `fr-en` | French → English | 66 MB | – |
| `fr-es` | French → Spanish | 67 MB | – |
| `fr-id` | French → Indonesian | 69 MB | – |
| `fr-ru` | French → Russian | 74 MB | – |
| `hi-en` | Hindi → English | 72 MB | – |
| `id-en` | Indonesian → English | 71 MB | – |
| `iir-en` | Persian → English | 71 MB | – |
| `it-en` | Italian → English | 72 MB | – |
| `ja-en` | Japanese → English | 68 MB | – |
| `ko-en` | Korean → English | 71 MB | – |
| `mul-en` | other languages → English | 62 MB | – |
| `pa-en` | Punjabi → English | 68 MB | – |
| `ru-en` | Russian → English | 70 MB | – |
| `tr-en` | Turkish → English | 72 MB | – |
| `ur-en` | Urdu → English | 70 MB | – |
| `zh-en` | Chinese → English | 74 MB | – |
