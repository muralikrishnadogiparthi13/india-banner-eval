# Would a shopkeeper post this? An India text-to-image eval

Can today's image models make a festive sale banner for a small Indian shop, with the offer written **correctly** in the shop's own language?

- **Results (leaderboard + every banner):** https://muralikrishnadogiparthi13.github.io/india-banner-eval/results.html
- **Rating app:** https://muralikrishnadogiparthi13.github.io/india-banner-eval/
- **Models:** OpenAI GPT Image 1, Google Gemini 2.5 Flash Image, Google Gemini 3.1 Flash Image, plus Ideogram 3.x as a text-rendering specialist.
- **Briefs:** 8 banners (saree shop, sweet shop, kirana, mobile accessories, tailor) in English (control), Hindi, Telugu, Tamil and Bengali. Exact prompts in `prompts.json`.
- **Judging:** native readers check whether the text is exactly right; each rater also says whether the shop could post it as-is and which one they would post. Models hidden, order shuffled per rater.

## Headline

On the 7 Indian-language briefs, Gemini 3.1 Flash Image was the only model with any banner a native reader called fully correct (14 of 14 ratings). The other three got 0 of 14 each, even though GPT Image 1 and Ideogram were fine on the English version of the same brief.

| Model | Post-ready, Indian languages | Post-ready, all | Picked |
|---|---|---|---|
| Gemini 3.1 Flash Image | 79% | 76% | 17 of 21 |
| GPT Image 1 | 0% | 24% | 1 of 21 |
| Ideogram 3.x | 0% | 10% | 3 of 21 |
| Gemini 2.5 Flash Image | 0% | 0% | 0 of 21 |

Post-ready = text fully correct AND the rater would post it as-is. 8 raters, 84 banner ratings; small sample, read it as a strong signal, not a benchmark.

## Files

- `ratings_anonymised.csv`: every rating (rater ids only).
- `model_mapping.json`: blind banner code → model.
- `prompts.json`, `briefs.json`: exact prompts and the intended text.
- `img/`: all 32 banners at 1024px.

Made by Murali Krishna Dogiparthi.
