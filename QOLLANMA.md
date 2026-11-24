# Saytni ishga tushirish va yangilash bo'yicha qo'llanma

Sayt **butunlay bepul**: GitHub Pages'da joylashadi (hosting — 0 so'm), tahrirlash Pages CMS orqali (0 so'm). Dasturlash bilish shart emas.

Natijada manzilingiz shunday bo'ladi: `https://SIZNING-NOMINGIZ.github.io`

---

## 1-qadam. GitHub akkaunt ochish (5 daqiqa)

1. https://github.com/signup ga kiring.
2. Foydalanuvchi nomini tanlang. **Bu nom sayt manzilingiz bo'ladi**, shuning uchun professional nom tanlang, masalan: `toshtemirov` yoki `btoshtemirov`.
3. Emailingizni tasdiqlang.

## 2-qadam. Sayt fayllarini yuklash (5 daqiqa)

1. Yuqori o'ng burchakdagi **+** → **New repository** ni bosing.
2. **Repository name** ga aynan shuni yozing: `SIZNING-NOMINGIZ.github.io`
   (masalan, nomingiz `toshtemirov` bo'lsa: `toshtemirov.github.io`).
3. **Public** ni tanlang → **Create repository**.
4. Ochilgan sahifada **uploading an existing file** havolasini bosing.
5. Men bergan ZIP faylni kompyuteringizda oching (Extract). Ichidagi **barcha fayl va papkalarni** brauzer oynasiga sudrab tashlang.
   - Diqqat: `.pages.yml` fayli "yashirin" bo'lishi mumkin. Windows'da: Explorer → View → **Hidden items** ni yoqing. Mac'da: `Cmd + Shift + .`
6. Pastdagi **Commit changes** tugmasini bosing.

## 3-qadam. Saytni yoqish (2 daqiqa)

1. Repozitoriyada **Settings** → chap menyuda **Pages**.
2. **Source**: `Deploy from a branch`, **Branch**: `main`, papka `/ (root)` → **Save**.
3. 1–2 daqiqadan so'ng sayt `https://SIZNING-NOMINGIZ.github.io` manzilida ochiladi.

## 4-qadam. Sayt manzilini sozlash (1 daqiqa, faqat bir marta)

1. Repozitoriyada `_config.yml` faylini oching → qalamcha (✏️ Edit) belgisini bosing.
2. `url: "https://USERNAME.github.io"` qatorida `USERNAME` o'rniga o'z nomingizni yozing.
3. **Commit changes**. Bu Google va AI tizimlari uchun to'g'ri havolalar yaratadi.

---

## Saytni o'zingiz yangilash — Pages CMS (forma orqali, kodsiz)

1. https://app.pagescms.org ga kiring → **Sign in with GitHub**.
2. Ruxsat so'ralganda `SIZNING-NOMINGIZ.github.io` repozitoriyasiga ruxsat bering.
3. Repozitoriyani tanlang → chap menyuda **"Mening ma'lumotlarim (CV)"**.
4. Kerakli maydonni o'zgartiring va **Save** bosing. 1–2 daqiqada saytda yangilanadi.

### Tez-tez bajariladigan ishlar

| Nima qilmoqchisiz | Qayerda |
|---|---|
| Yangi maqola qo'shish | **Maqolalar** → **Add an entry** → uni ro'yxatning **eng yuqorisiga** suring. Turi: `journal`, `chapter` yoki `in-press` |
| "In press" maqola chiqdi | O'sha maqolani oching → Turi: `journal`, DOI va sahifalarni yozing |
| Yangi ish joyi | **Ish tajribasi** → yangi yozuv, eski ishning "Tugagan" maydonini to'ldiring |
| h-index yoki raqamlar | **Raqamlar (bosh sahifa kartasi)** |
| Rasm qo'yish | **Rasm** maydoni → rasm yuklang (kvadrat, kamida 400×400 px) |
| Yangi CV PDF | **CV fayli (PDF)** maydoni → yangi faylni yuklang |
| ORCID, Google Scholar va h.k. | **Ilmiy profillar havolalari** |

Bo'sh qoldirilgan maydon saytda ko'rinmaydi. Har bir o'zgarish GitHub'da saqlanadi — xato qilsangiz, eski holatga qaytarish mumkin (repozitoriya → **Commits**).

**Muhim:** saytning barcha matni va JSON-LD (AI uchun ma'lumot), `llms.txt` fayli **avtomatik ravishda** shu ma'lumotlardan yaratiladi. Bir joyda o'zgartirsangiz, hammasi yangilanadi.

---

## AI va Google sizni topishi uchun (juda muhim)

Sayt ichida bularning hammasi allaqachon bor: tuzilgan ma'lumot (schema.org Person + har bir maqola), `llms.txt` (AI uchun maxsus profil), `robots.txt` (ChatGPT, Claude, Perplexity, Gemini botlariga ruxsat), `sitemap.xml`.

Siz qilishingiz kerak bo'lgan ishlar:

1. **Ilmiy profillar havolalarini qo'shing** (ORCID, Google Scholar, Scopus Author ID, ResearchGate, MathSciNet, zbMATH). AI sizni boshqa "Toshtemirov"lardan aynan shu havolalar orqali ajratadi.
2. **Teskari havola qo'ying:** ORCID, Google Scholar, LinkedIn, ResearchGate profillaringizdagi "Website" maydoniga sayt manzilini yozing. Ikki tomonlama bog'lanish — eng kuchli signal.
3. **Google Search Console:** https://search.google.com/search-console → saytni qo'shing → `sitemap.xml` ni yuboring. **Bing Webmaster Tools** ga ham qo'shing (https://www.bing.com/webmasters) — ChatGPT qidiruvi Bing'dan foydalanadi.
4. **Rasmingizni qo'shing** — profilni ishonchli qiladi.
5. Ma'lumotlarni yangilab turing: AI eng so'nggi va izchil ma'lumotni afzal ko'radi.

---

## O'z domeningiz (ixtiyoriy, pullik)

`toshtemirov.com` kabi domen yiliga taxminan $10–15. Sotib olgach: repozitoriya → Settings → Pages → **Custom domain**. Keyin `_config.yml` dagi `url` ni yangi domenga o'zgartiring.
