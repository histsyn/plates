# LeeHysan images — manifest & gate log

All production plates were read back by the session model's own eyes at their
FINAL bytes on 2026-11-16 (the §6B gate). The ksyp (工商日報) pages were
downloaded from the public viewer via the tailnet origin route
(`curl --resolve hkintexts.histsyn.com:443:100.116.224.127 …`, the viewer's
`imagePath` is JSON-escaped and must be unescaped). Newspaper items are
**column crops / article blocks** per the 2026-10-19 rule.

| File | What it shows | Source | Gate |
|---|---|---|---|
| `plate_murder_19280501.jpg` | The murder report: 工商日報 1928-05-01 p.6 — header 「第二張」; the portrait; the vertical headline 「利希慎被刺／連擊三槍／兇手未獲」; the report opening 「本港鉅商利希慎君, 於昨日下午一點二十分鐘…」 | https://hkintexts.histsyn.com/image-page/217559 | **PASS** |
| `plate_funeral_19280526.jpg` | The funeral report: 工商日報 1928-05-26 p.6 — 「利希慎出殯情形（本報特訊）」 + the recap + the ▲ sections (華人到送殯者/孝幃內之人物/西人到場送殯/軍樂隊之數目/學生列隊送殯…) | https://hkintexts.histsyn.com/image-page/217939 | **PASS** |
| `plate_estate_19281120.jpg` | The estate report: 工商日報 1928-11-20 p.14 — 「港聞二」 + 「利希慎之遺產」 + 「遺二百七十一萬六千四百元」 + the arithmetic (gross $4,461,145.85 / debts $1,744,751 / 八厘遺產稅并利息 $217,312) | https://hkintexts.histsyn.com/image-page/219731 | **PASS** |
| `plate_shareholders_19290412.jpg` | The shareholders' notice: 工商日報 1929-04-12 p.2 — 「利希慎夫人黃蘭芳嫂鑒」 + the 裕成公司股東團's plea + 「裕成公司股東團上」; dated 己巳年三月初三日 | https://hkintexts.histsyn.com/image-page/220417 | **PASS** |
| `fb_portrait_19280501.jpg` | **The FB single image** — the newspaper's own portrait (「利希慎君遺像」) from the murder report page, with its printed caption row included (crop re-cut 2026-11-17: the first crop ended at raw y=2162 and cut the caption's lower half; the caption sits at raw y 2152–2182), despeckled (median 3) and 3× | crop of /image-page/217559 | **PASS** (re-gated 2026-11-17 at the final bytes) |
| `fb_closure_notice_19280524.jpg` | **[W1]** 澳門裕成鴉片公司結束要告白 — the Macao Yue Sing Opium Company's winding-up notice, dated 戊辰年四月初三日 (21 May 1928), printed 華字日報 24 May 1928 3rd sheet p.2; signed 高露雲律師樓 (Wilkinson & Grist). Wikimedia Commons, Public domain (PD Hong Kong / PD-1996); uploaded 2023. Credit line for use: 「圖片：澳門裕成鴉片公司結束要告白，《香港華字日報》1928年5月24日；Wikimedia Commons，公有領域」 | https://commons.wikimedia.org/wiki/File:澳門裕成鴉片公司因利希慎斃命結業通告.jpg | **PASS** |
| `raw/` | The untouched downloads: `ksyp19280501_p6_murder`, `ksyp19280526_p6_funeral2`, `ksyp19280526_p8_funeral` (the flowers item — NOT used as the funeral plate), `ksyp19281120_p14_estate`, `ksyp19290412_p2_shareholders` | viewer `/img/<uuid>` | — |
| `work/` | Probe crops and previews used during the locating/gate passes (disposable) | — | — |

Gaps: **no PD portrait photograph outside the press** was located (Wikimedia
Commons holds only modern Hysan Place/Lee Garden Road photographs); the press
portrait (`fb_portrait_19280501.jpg`) is the image of record. English-press
items for 1928 (China Mail / Daily Press / Telegraph) have **no image scans**
(the chinamail image series ends 1919) — their citations are text-series only.
