# ChineseNaming_Qing / images — plate manifest

Thread: 清代香港對「中國人」的稱呼 (what the Chinese of Hong Kong were called, 1841–1912).
**Production plates = the `_hl` files** — each carries amber highlight boxes seated on the quoted words and was **read back by eye at its final bytes** (the §6B hard gate; first pass 2026-10-29, boxed re-make and re-read the same day after the user's catch that the first set shipped as raw scans).

| Production file | What it shows (verified by eye) | Viewer link (source of record) | What the amber box(es) wrap |
|---|---|---|---|
| `plate_1858_proclamation_hl.jpg` | Gazette 31 July 1858 — the Chinese column of Bowring's proclamation | https://hkintexts.histsyn.com/image-page/1448108 | 「本港所居**漢人**甚衆」; 「勒令**漢人**回去之告示長紅改正」; 「**大清皇帝之罪民**」 (English side of the same notice: "compelling **the Chinese People** to leave this Colony") |
| `plate_1859_salepigs_hl.jpg` | Gazette, printed p. 215, April 1859 — the Cantonese Governor's anti-kidnapping proclamation | https://hkintexts.histsyn.com/image-page/1448275 | 「販賣出洋名曰**賣猪仔**，日久不得還鄉」 (printed 猪/曰 — scan-settled at zoom, `probe_pig_char.jpg`) + English "the **sale of pigs**" |
| `plate_1868_tangtze_ad_hl.jpg` | *China Mail*, 18 March 1868, printed p. 8 — the "**Chinese Advertisements.**" section (column crop, newspaper rule) | https://hkintexts.histsyn.com/image-page/1183549 | the printing-office ad block: 「刷印**唐字**另具一紙以備**唐人閱看**」(hand-painted box from the OCR box coordinates) |
| `plate_1879_formula_hl.jpg` | Gazette No. 21, 28 May 1879 — the bilingual formula leaf + the Chinese-passengers notice | https://hkintexts.histsyn.com/image-page/1477363 | "**Chinese portion of the Community**" block + 「**俾本港華人週知**」 column; "**Chinese Passengers**" block + 「**華人搭客**」 column |
| `plate_1881_address_hl.jpg` | Gazette, 23 April 1881, printed p. 276 — the congratulatory address | https://hkintexts.histsyn.com/image-page/1504953 | 「**闔港華人紳商**等敬頌」 column; 「**大清光緒七年**」＋日期; English "a congratulatory address by the **Chinese people, gentry and merchants**" |
| `plate_1892_asylum_hl.jpg` | Gazette, 6 February 1892, printed p. 120 — the Lunatic Asylum vacancy | https://hkintexts.histsyn.com/image-page/1539910 | 「**國家華民癲人院**現有**唐人管事**兼傳話一缺」 column |
| `plate_1899_convention_hl.jpg` | Gazette, 8 April 1899, printed p. 582 — the New Territories settlement (both printings on the leaf) | https://hkintexts.histsyn.com/image-page/1550072 | 「**大英國大皇帝**與**大清國大皇帝**訂立約章…」 columns, both copies |
| `plate_1854_diet_hl.jpg` *(supplementary; not wired as a paper figure)* | Gazette, 1854 (甲寅年四月初九日) — the gaol diet tender | https://hkintexts.histsyn.com/image-page/1447151 | 「每日**英人一名漢人一名**所用各項」 column; 「凡**漢人**每日粗米一斤半鹹魚或鮮魚二兩」 column |
| `plate_1879_directory_hl.jpg` *(supplementary; not wired as a paper figure)* | *Directory and Chronicle* 1879, printed p. 190 | https://hkintexts.histsyn.com/image-page/901222 | the "REGISTRAR GENERAL'S OFFICE / **華民政務司**" section + the marriages section below it |

## Notes

* **Raw scans** are kept in `raw/` (file names `raw_<image-id>.jpg`), and the unboxed tool outputs as `<stem>.jpg`; the boxed `_hl` files are the production set.
* Working verification artefacts: `k4_zoom3.jpg` / `k4_zoom4.jpg` (the 1879 address's 「…之本土艮民…」 glyph — ambiguous; the phrase is never quoted; see the notes, K4); `probe_pig_char.jpg` (the 1859 猪/曰 settlement).
* **The inscriptions are NOT plated**: the `inscriptions-image` series is login-gated (no `imagePath` served) and the 香港碑銘彙編 is a modern compilation; the stone texts cited in the thread (1727 burner 「大清國廣東廣州新安縣泰坑本鄉」; 1904/1911 同胞 couplets; 1910 華商燕梳) are quoted from the text series, the images used for verification only, never republished.
* **Tool notes (this thread's lessons, recorded in `tools/scan_highlights.py`):** the viewer fetch falls back to the tailnet route (`--resolve hkintexts.histsyn.com:443:<ES host>`) when Cloudflare answers 403; and the ink-band seat step is guarded — a tall vertical-column box must not be silently collapsed into a single ink band (if a >250px box would shrink below 40%, the original coordinates are kept). The 1858/1881 boxes had been silently collapsed before the guard; all plates were re-run and re-read after it.
* Hosted copies: `https://histsyn.github.io/plates/ChineseNaming_Qing/images/<file>` (pushed 2026-10-29, md5-verified against these files).
* All sources are Hong Kong Government Gazettes / the *China Mail* / the *Directory and Chronicle* of the 1850s–1890s — public-domain by age.
