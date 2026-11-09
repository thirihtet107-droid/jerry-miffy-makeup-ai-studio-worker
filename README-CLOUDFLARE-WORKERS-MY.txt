JERRY MIFFY MAKEUP AI STUDIO — CLOUDFLARE WORKERS BUILD

ဤ ZIP သည် Cloudflare Workers အတွက် ပြန်လည်ဖွဲ့စည်းထားသော project ဖြစ်သည်။
မူလ Pages Functions folder ကို Worker entry point (src/index.js) အဖြစ် ပေါင်းစည်းထားသည်။

API routes:
- POST /api/consult
- POST /api/preview

Deploy အတွက်:
1. ZIP ကို Extract လုပ်ပါ။
2. Cloudflare Dashboard → Workers & Pages → Workers → Create → Import a repository (GitHub) သို့မဟုတ် Wrangler CLI ဖြင့် project ကို deploy လုပ်ပါ။
3. Worker project root တွင် wrangler.toml ရှိရမည်။
4. Worker Settings → Variables and Secrets တွင် GEMINI_API_KEY ကို Secret အဖြစ်ထည့်ပါ။
5. Deploy ပြီးနောက် Website ကိုဖွင့်ပြီး Analyze / Preview စမ်းပါ။

သတိပြုရန်:
- ZIP ကို Workers dashboard ထဲက static asset upload တစ်ခုတည်းအဖြစ်တင်ခြင်းမဟုတ်ဘဲ Worker script နှင့် assets အဖြစ် deploy လုပ်ရမည်။
- GEMINI_API_KEY ကို public HTML/JS ထဲ မထည့်ပါနှင့်။
- ယခင် Netlify/Pages website ကို မပြောင်းလဲပါ။
- Gemini model/API availability, quota နှင့် billing ကြောင့် API response error သီးခြားဖြစ်နိုင်သည်။
