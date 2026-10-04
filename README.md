# Would a shopkeeper post this? An India text-to-image eval

A small, focused evaluation: can today's image models make a festive sale banner for a small Indian shop, with the offer written **correctly** in the shop's own language?

- **Rating app:** https://muralikrishnadogiparthi13.github.io/india-banner-eval/
- **Models:** OpenAI GPT Image 1, Google Gemini 2.5 Flash Image, Google Gemini 3.1 Flash Image, plus Ideogram 3.0 as a text-rendering specialist.
- **Briefs:** 8 banners (saree shop, sweet shop, kirana, mobile accessories, tailor) in English (control), Hindi, Telugu, Tamil and Bengali. Exact prompts in `prompts.json`.
- **Judging:** native readers check whether the text is exactly right; everyone says whether the shop could post it as-is and which one they would post. Models are hidden and the order is shuffled per rater.

Image files are named with random codes so raters can't tell which model made what. The code-to-model mapping is published after the ratings close.

Made by Murali Krishna Dogiparthi.
