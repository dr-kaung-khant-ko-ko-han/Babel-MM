# Babel နှင့် Polyglossia — LaTeX ဘာသာစုံစာစီစာရိုက်လမ်းညွှန်
## မြန်မာဘာသာပြန် (Myanmar/Burmese Translation)

---

# အပိုင်း ၁ — Babel (ဘေဘယ်) အသုံးပြုသူလမ်းညွှန်

**မူကွဲ 25.16 | ၂၀၂၅/၁၁/၂၃**

**ဒေသအလိုက်ပြောင်းလဲခြင်းနှင့် နိုင်ငံတကာပြုခြင်း (Localization and Internationalization)**

| | |
|---|---|
| **Javier Bezos** — လက်ရှိထိန်းသိမ်းသူ | **ယူနီကုဒ် (Unicode)** — LuaTeX, pdfTeX, XeTeX |
| **Johannes L. Braams** — မူရင်းတီထွင်သူ | **TeX** |

---

## နိဒါန်း (Preface)

**ဤစာရွက်စာတမ်းသည် အဘယ်အကြောင်းအရာကို ဖော်ပြသနည်း?**
ဤအသုံးပြုသူလမ်းညွှန်သည် LATEX နှင့် LuaTeX, pdfTeX, XeTeX တို့တွင် babel package ဖြင့် နိုင်ငံတကာပြုခြင်း (internationalization) နှင့် ဒေသအလိုက်ပြောင်းလဲခြင်း (localization) အကြောင်း အာရုံစိုက်ဖော်ပြထားပါသည်။ e-Plain နှင့် pdf-Plain TEX တို့နှင့် အသုံးပြုခြင်းဆိုင်ရာ မှတ်စုအချို့လည်း ပါဝင်ပါသည်။

**အခြေခံအင်္ဂါရပ်များကိုသာ လေ့လာလိုပါသည်။**
ပထမဆုံး ဆပ်ခန်းငယ်များ (၁.၁-၁.၆) သည် ဘာသာစကားတစ်ခုကို တင်ရန် နည်းလမ်းများကို ဖော်ပြထားပြီး၊ များသောအားဖြင့် သင်လိုအပ်သမျှ ဖြစ်ပါသည်။

**လမ်းညွှန်စာအုပ်များကို မကြိုက်ပါ။ နမူနာဖိုင်များကို ပို၍နှစ်သက်ပါသည်။**
ဤလမ်းညွှန်တွင် ဥပမာများနှင့် အကြံပြုချက်များ များစွာပါဝင်သော်လည်း၊ GitHub တွင် နမူနာဖိုင်များ များစွာရှိပါသည်။

**နောက်ဆုံးပြောင်းလဲမှုများကိုသာ စိတ်ဝင်စားပါက?**
ဗားရှင်း ၃.၈ နှင့် ဆက်စပ်သော ပြောင်းလဲမှုများနှင့် အင်္ဂါရပ်အသစ်များကို X.XX ဖြင့် အထူးပြုထားပြီး (※ သည် babel site သို့ လင့်ခ်ဖြစ်သည်)၊ babel site တွင် နောက်ဆုံးဗားရှင်းများအတွက် မှတ်စုအချို့ရှိပါသည်။

**ကူညီနိုင်ပါသလား?**
ဟုတ်ကဲ့! GitHub တွင် babel ၏ တိုးတက်မှုကို လိုက်ကြည့်နိုင်ပြီး အကြံပြုချက်များပြုလုပ်နိုင်ပါသည်။ ၎င်းကို fork လုပ်၍ pull requests များ လွတ်လပ်စွာ ပြုလုပ်နိုင်ပါသည်။

**ကျွန်ုပ်အတွက် အလုပ်မဖြစ်ပါ!**
tex.stackexchange ကဲ့သို့သော ဖိုရမ်များတွင် အကူအညီတောင်းနိုင်ပါသည်။ bug တစ်ခုကို တွေ့ရှိပါက၊ GitHub တွင် သတင်းပို့ရန် အထူးတောင်းဆိုပါသည်။

---

## ၁. အခြေခံအသုံးပြုသူ အင်တာဖေ့စ် (The Basic User Interface)

babel ဖြင့် ဘာသာစကားတစ်ခုကို တင်ရန် နည်းလမ်း နှစ်မျိုးရှိပါသည် -

**၁. ဂန္ထဝင်နည်းလမ်း (Classical way)**: ldf တိုးချဲ့မှုပါသော ဖိုင်တွင် အများအားဖြင့် သီးခြားပါဝင်သော ကြေညာချက်များအပေါ် အခြေခံထားသည်။

**၂. ခေတ်မီနည်းလမ်း (Modern way)**: ဖော်ပြချက် ini ဖိုင်များအပေါ် အခြေခံထားသော လုံးဝအသစ်သော ယန္တရားပေါ် တည်ဆောက်ထားသည်။

'ရိုးရာ' ဆိုသည်မှာ ခေတ်နောက်ကျ သို့မဟုတ် အသုံးမဝင်ဟု အဓိပ္ပါယ်မရပါ။ တကယ်တော့ ldf ဖိုင်ရှိသော ဘာသာစကားအများစုတွင် ဤသည်မှာ အကြံပြုထားသော နည်းလမ်းဖြစ်ပါသည်။

အခြေခံအားဖြင့်၊ သင်လိုအပ်သည်မှာ -

- babel ကို မည်သည့်ဘာသာစကား သို့မဟုတ် ဘာသာစကားများ လိုအပ်ကြောင်း ပြောပြပါ။
- လက်တင်မဟုတ်သော စာလုံးပုံစံများနှင့် Unicode အင်ဂျင်များဖြင့် (luatex သည် နှစ်သက်ရသော တစ်ခုဖြစ်သည်)၊ သင့်လျော်သော ဖောင့်တစ်ခု ရွေးချယ်ပါ။
- ဘာသာစကားများစွာပါသော စာရွက်စာတမ်းများတွင်၊ စာသားပိုင်းတွင် ဘာသာစကားကို ပြောင်းပါ။

### ၁.၁ ဘာသာစကားတစ်မျိုးတည်းစာရွက်စာတမ်းများ — ဂန္ထဝင်နည်းလမ်း (Monolingual documents: the 'classical' way)

အများအားဖြင့် ဘာသာစကားတစ်မျိုးတည်းသာ လိုအပ်ပြီး၊ LATEX တွင် package ကို optional argument အဖြစ် ထိုဘာသာစကားကို ဖြတ်ပေးရုံသာ လိုအပ်ပါသည်။

ဥပမာ -
```
\DocumentMetadata{lang=en-GB}
\documentclass{article}
\usepackage{babel}
```

ဤသို့သတ်မှတ်ခြင်းဖြင့် british ကို babel ၏ အဓိကဘာသာစကားအဖြစ် သတ်မှတ်ပေးပါမည်။

**ရိုးရာ TEX အင်ဂျင်များအတွက် နမူနာ -**
```
\documentclass{article}
\usepackage[T1]{fontenc}
\usepackage[french]{babel}
\begin{document}
    Plus ça change, plus c'est la même chose!
\end{document}
```

**LuaTeX/XeTeX ဖြင့် ရုရှားဘာသာဖြင့် နမူနာ -**
```
\documentclass[russian]{article}
\usepackage{babel}
\babelfont{rm}{DejaVu Serif}
\begin{document}
Россия, находящаяся на пересечении множества культур...
\end{document}
```

**မှတ်ချက်များ -**
- babel သည် ဖောင့်အရွယ်အစား၊ ဒေါင်လိုက်တည်နေရာချထားမှု သို့မဟုတ် မျဉ်းအမြင့်တွင် မည်သည့် ပြန်လည်ညှိနှိုင်းမှုမျှ default အားဖြင့် မပြုလုပ်ပါ။
- hyperref ဖြင့် PDF စာရွက်စာတမ်း ဘာသာစကားကို `\usepackage[pdflang=es-MX]{hyperref}` ဖြင့် သတ်မှတ်နိုင်ပါသည်။

**ပြဿနာဖြေရှင်းခြင်း (Troubleshooting) -**

*Package inputenc Error*: အဖြစ်များသော ပြဿနာမှာ input encoding ၏ မှားယွင်းသော သတ်မှတ်ချက်ဖြစ်သည်။ သင့် editor တွင် encoding ကို UTF-8 သို့ သတ်မှတ်ပါ။

*Package babel Error: Unknown language 'LANG'*: အဖြစ်များဆုံးအကြောင်းရင်းမှာ သင်သည် ဘာသာစကားတစ်ခုကို ရွေးချယ်ခေါ်ယူပြီးနောက် option list မှ ဖယ်ရှားလိုက်ခြင်းကြောင့်ဖြစ်သည်။ aux ဖိုင်ကို ဖျက်ပြီး ပြန်စမ်းကြည့်ပါ။

*No hyphenation patterns were preloaded*: စာရွက်စာတမ်းကို စာစီနိုင်မည်ဖြစ်သော်လည်း ဝဏ္ဏခွဲခြင်း (hyphenation) မှန်ကန်မည်မဟုတ်ပါ။

### ၁.၂ ဘာသာစကားတစ်မျိုးတည်းစာရွက်စာတမ်းများ — ခေတ်မီနည်းလမ်း (Monolingual documents: the 'modern' way)

ldf ယန္တရားဖြင့် မပံ့ပိုးသော ဘာသာစကားများအတွက် `provide=*` option ကို အသုံးပြုနိုင်ပါသည်။

**ဂျော်ဂျီယာဘာသာအတွက် နမူနာ -**
```
\documentclass{book}
\usepackage[georgian, provide=*]{babel}
\babelfont{rm}[Renderer=Harfbuzz]{DejaVu Sans}
\begin{document}
\tableofcontents
\chapter{სამზარეულო და სუფრის ტრადიციები}
ქართული ტრადიციული სამზარეულო...
\end{document}
```

**တရုတ်ဘာသာအတွက် နမူနာ -**
```
\usepackage[chinese]{babel}
\babelfont{rm}{FandolSong}
```

### ၁.၃ အများအားဖြင့် ဘာသာစကားတစ်မျိုးတည်းစာရွက်စာတမ်းများ — နှောင့်နှေးဖွင့်ခြင်း (Mostly monolingual documents: lazy loading)

ဘာသာစကားမျိုးစုံအတွက် ရည်ရွယ်ထားသော်လည်း အများအားဖြင့် ဘာသာစကားတစ်မျိုးတည်းသာ အသုံးပြုသော စာရွက်စာတမ်းများအတွက် 'lazy loading' ကို အသုံးပြုနိုင်ပါသည်။

```
\documentclass{book}
\usepackage{babel}
```

ထို့နောက် လိုအပ်သောဘာသာစကားကို `\selectlanguage` ဖြင့် ပြောင်းလဲအသုံးပြုနိုင်ပါသည်။

### ၁.၄ ဘာသာစကားမျိုးစုံစာရွက်စာတမ်းများ — ဂန္ထဝင်နည်းလမ်း (Multilingual documents: the 'classical' way)

```
\usepackage[french,english]{babel}
```

ဤတွင် နောက်ဆုံးဘာသာစကား (english) သည် အဓိကဘာသာစကားဖြစ်သည်။ စာသားထဲတွင် `\selectlanguage{french}` ဖြင့် ဘာသာပြောင်းနိုင်သည်။

```
\selectlanguage{german}
```
```
\foreignlanguage{french}{français}
```

### ၁.၅ ဘာသာစကားမျိုးစုံစာရွက်စာတမ်းများ — ခေတ်မီနည်းလမ်း (Multilingual documents: the 'modern' way)

Option သုံးမျိုး -

- `provide=*` - အဓိကဘာသာစကားအတွက်သာ ခေတ်မီနည်းလမ်း
- `provide+=*` - အဓိကဘာသာစကားအတွက် ဂန္ထဝင်နည်းလမ်း၊ ကျန်ဘာသာများအတွက် ခေတ်မီနည်းလမ်း
- `provide*=*` - ဘာသာစကားအားလုံးအတွက် ခေတ်မီနည်းလမ်း

### ၁.၆ - ၁.၇ ပံ့ပိုးထားသော ဘာသာစကားများ (Supported languages)

babel သည် ဘာသာစကားများစွာကို ပံ့ပိုးထားပြီး၊ ဘာသာစကားတစ်ခုချင်းစီတွင် သီးသန့်ရွေးချယ်စရာများ ရှိပါသည်။ အဓိကဘာသာစကားများမှာ - afrikaans, arabic, basque, catalan, chinese, czech, danish, dutch, english (ဗားရှင်းအမျိုးမျိုး), finnish, french, german (ဗားရှင်းအမျိုးမျိုး), greek, hebrew, hindi, hungarian, italian, japanese, korean, latin, norwegian, polish, portuguese, romanian, russian, spanish, swedish, thai, turkish, ukrainian, vietnamese စသည်တို့ဖြစ်သည်။

### ၁.၈ ယူနီကုဒ်အင်ဂျင်များတွင် ဖောင့်များ (Fonts in Unicode engines)

`\babelfont` ညွှန်ကြားချက်ကို အသုံးပြု၍ ဘာသာစကားအလိုက် ဖောင့်များသတ်မှတ်နိုင်သည် -

```
\babelfont{rm}{DejaVu Serif}
\babelfont{sf}{DejaVu Sans}
\babelfont{tt}{DejaVu Sans Mono}
```

ဘာသာစကားအလိုက် ဖောင့်သတ်မှတ်ခြင်း -
```
\babelfont[Russian]{rm}{Noto Serif}
\babelfont[Greek]{rm}{Noto Serif}
```

### ၁.၉ အခြေခံဘာသာစကားရွေးချယ်ကိရိယာများ (Basic language selectors)

**\selectlanguage** - စာသားပိုင်းကြီးများအတွက် အသုံးပြုသည် -
```
\selectlanguage{german}
```

**\foreignlanguage** - စာပိုဒ်တိုများအတွက် အသုံးပြုသည် -
```
\foreignlanguage[date]{polish}{\today}
```

### ၁.၁၀ အရန်ဘာသာစကားရွေးချယ်ကိရိယာများ (Auxiliary language selectors)

**otherlanguage** environment - selectlanguage အတိုင်းဖြစ်သော်လည်း space များကို လျစ်လျူရှုသည်။

**otherlanguage*** environment - \foreignlanguage အတိုင်းဖြစ်သော်လည်း environment အဖြစ်အသုံးပြုနိုင်သည်။

---

## ၂. ဘာသာစကားဖွင့်ခြင်းနှင့်ရွေးချယ်ခြင်းအကြောင်း ထပ်မံ (More on language loading and selection)

### ၂.၁ ကိရိယာအချို့ (A few tools)

```
\babelprovide[import, language.Default]{burmese}
```

### ၂.၂ ဘာသာစကားအချက်အလက်များကို ရယူခြင်း (Accessing language info)

```
\languagename   % လက်ရှိဘာသာစကားအမည်
\localename     % ဒေသဆိုင်ရာအမည်
\the\language  % လက်ရှိ hyphenation pattern နံပါတ်
```

### ၂.၃ Package Options

babel package အတွက် ရွေးချယ်စရာများ -
- `main=` - အဓိကဘာသာစကားကို သတ်မှတ်ခြင်း
- `headfoot=` - ခေါင်းစီးနှင့်အောက်ခြေစာများအတွက် ဘာသာစကား
- `bidi=` - ညာမှဘယ်စာရေးစနစ်အတွက် (basic, basic-r, bidi, default)
- `layout=` - အပြင်အဆင်ဆိုင်ရာ ပြုပြင်ချက်များ

### ၂.၄ The base option

```
\usepackage[english, base]{babel}
```

### ၂.၅ provide နှင့် \babelprovide

```
\babelprovide[import=my, language.Default]{burmese}
```

### ၂.၆ BCP 47 Tags အပေါ်အခြေခံ၍ ရွေးချယ်ခြင်း (Selection based on BCP 47 tags)

```
\usepackage[english]{babel}
\babelprovide[import, language.Default]{my}
```

---

## ၃. ဘာသာစကားကို အံဝင်ခွင်ကျဖြစ်အောင်ပြုလုပ်ခြင်း၊ စိတ်ကြိုက်ပြုပြင်ခြင်းနှင့် ပြုပြင်မွမ်းမံခြင်း (Tailoring, customizing and modifying a language)

### ၃.၁ Captions

```
\addto\captionsburmese{\renewcommand{\prefacename}{နိဒါန်း}}
\addto\captionsburmese{\renewcommand{\chaptername}{အခန်း}}
\addto\captionsburmese{\renewcommand{\contentsname}{မာတိကာ}}
```

### ၃.၂ Modifiers

```
\addto\extrasburmese{\hyphenrules{burmese}}
```

### ၃.၃ Language attributes

```
\babelprovide[attributes]{burmese}
```

### ၃.၄ Casing

```
\MakeUppercase, \MakeLowercase
```

### ၃.၅ ini ဖိုင်များတွင် တန်ဖိုးများပြုပြင်ခြင်းနှင့်ထည့်သွင်းခြင်း

### ၃.၆ Hooks

```
\babelprehyphenation{burmese}{...}{...}
\babelposthyphenation{burmese}{...}{...}
```

### ၃.၇ ဖိုင်များကို စီမံခန့်ခွဲခြင်း (Manage auxiliary files)

### ၃.၈ Code based on the selector

### ၃.၉ Presets

---

## ၄. ဘာသာစကားတစ်ခုကို ဖန်တီးခြင်း (Creating a language)

babel တွင် ဘာသာစကားအသစ်တစ်ခုကို ဖန်တီးရန် ldf သို့မဟုတ် ini ဖိုင်များကို အသုံးပြုနိုင်သည်။

အခြေခံ ini ဖိုင်ပုံစံ -
```
[identification]
    name.local = မြန်မာ
    tag.bcp47 = my
    script.name = Myanmar
[chars]
    alphabet = ကခဂဃငစဆဇဈဉဋဌဍဎဏတထဒဓနပဖဗဘမယရလဝသဟဠအ
[typography]
    after.indent = 0pt
[captions]
    preface = နိဒါန်း
    chapter = အခန်း
    contents = မာတိကာ
    index = အညွှန်း
    figure = ရုပ်ပုံ
    table = ဇယား
```

---

## ၅. ဒေသဆိုင်ရာအင်္ဂါရပ်များ (Locale features)

### ၅.၁ ဝဏ္ဏခွဲခြင်းနှင့် မျဉ်းကျိုးခြင်း — ၁. ညွှန်ကြားချက်များ (Hyphenation and line breaking — 1. Commands)

babel သည် မျဉ်းကျိုးစည်းမျဉ်း (line breaking rules) သုံးမျိုးကို ကိုင်တွယ်သည် -
1. အနောက်တိုင်း (Western / LGC group)
2. အရှေ့တောင်အာရှ (ထိုင်း စသည်)
3. CJK (တရုတ်/ဂျပန်/ကိုရီးယား)

```
\babelhyphenation{Wal-hal-la Dar-bhan-ga}
\babelpatterns[thai]{ศึก2ษา}
```

### ၅.၂ ဝဏ္ဏခွဲခြင်းနှင့် မျဉ်းကျိုးခြင်း — ၂. 'Provide' options

### ၅.၃ အတိုကောက်များ — ၁. ညွှန်ကြားချက်များ (Shorthands — 1. Commands)

```
\useshorthands{"}
\defineshorthand{"-}{\textormath{\nobreak-\hyphenpenalty\@M}{-}}
```

### ၅.၄ အတိုကောက်များ — ၂. Package options

### ၅.၅ ဂဏန်းများနှင့် ရေတွက်ကိရိယာများ (Digits and counters)

### ၅.၆ ရက်စွဲများ (Dates)

```
\today  % လက်ရှိရက်စွဲကို လက်ရှိဘာသာစကားဖြင့် ပြသည်
```

### ၅.၇ ဒေသဆိုင်ရာအင်္ဂါရပ်များအတွက် နောက်ထပ်စာသားများ

### ၅.၈ Bidi (ညာမှဘယ်စာရေးစနစ်)

bidi = bidirectional text အတွက် options များ -

- `bidi=basic` - LuaTeX အတွက်
- `bidi=bidi` - XeTeX အတွက်

```
\usepackage[bidi=basic, layout=counters tabular]{babel}
```

### ၅.၉ မျက်နှာပြင်အပြင်အဆင် (Layout)

`layout` option ဖြင့် ဘာသာစကားအလိုက် မျက်နှာပြင်အပြင်အဆင်ကို ပြုပြင်နိုင်သည် -
- counters, tabular, lists, sectioning, footnotes, etc.

### ၅.၁၀ စာပိုဒ်ခွဲများ (Floats and footnotes)

```
\BabelFootnote{\footnote}{\localename}{}{}
```

### ၅.၁၁ LuaTeX ရှိ ယူနီကုဒ်စာလုံးသွင်ပြင်လက္ခဏာများ (Unicode character properties in luatex)

```
\babelcharproperty{`¿}{mirror}{`?}
\babelcharproperty{`-}{direction}{l}
```

### ၅.၁၂ babel အင်္ဂါရပ်များကို ချိန်ညှိခြင်း (Tweaking some babel features)

```
\babeladjust{linebreak.sea=off}
\babeladjust{bidi.math=off}
```

---

## ၆. ini ဖိုင်များ (ini files)

ini ဖိုင်များသည် ဘာသာစကားသတ်မှတ်ချက်များကို သိမ်းဆည်းရန် အသုံးပြုသော ခေတ်မီယန္တရားဖြစ်သည်။

ini ဖိုင်ကဏ္ဍများ -
1. **identification** - ဘာသာစကားအမည်နှင့် BCP 47 tag
2. **chars** - အက္ခရာများနှင့် စာလုံးပုံစံများ
3. **typography** - စာစီစာရိုက်ဆိုင်ရာ သတ်မှတ်ချက်များ
4. **captions** - စာတန်းများ
5. **date** - ရက်စွဲပုံစံ
6. **numbers** - ဂဏန်းများ

---

## ၇. Fonts with Latin and non-Latin scripts

```
\babelfont[Burmese]{rm}{Noto Sans Myanmar}
\babelfont[Burmese]{sf}{Noto Sans Myanmar}
```

---

## ၈. Babel and other packages

### ၈.၁ hyperref

```
\usepackage[pdflang=my-MM]{hyperref}
```

### ၈.၂ fontenc နှင့် inputenc

```
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}
```

### ၈.၃ bidi package

### ၈.၄ Other packages

---

## ၉. ပံ့ပိုးခြင်း (Contributing)

ဘာသာစကားအသစ်တစ်ခုကို မည်သို့ပံ့ပိုးနိုင်မည်နည်း? အပိုဒ် ၉.၁ ကို ကြည့်ပါ။

```
\babelprovide[import=my, language.Default]{burmese}
```

ထို့နောက် ini ဖိုင်တွင် လိုအပ်သော သတ်မှတ်ချက်များကို ထည့်သွင်းနိုင်ပါသည်။

---

## ၁၀. ကျေးဇူးတင်လွှာ (Acknowledgements)

babel ၏ ဖွံ့ဖြိုးတိုးတက်မှုအစောပိုင်းတွင် Bernd Raichle မှ အကြံပြုချက်များစွာနှင့် Michel Goossens မှ ဘာသာစကားများစွာအတွက် ပံ့ပိုးမှုများ ပေးအပ်ခဲ့ပါသည်။ Salim Bou, Ulrike Fischer, Loren Davis နှင့် Udi Fogiel တို့မှ အရေးပါသော ပံ့ပိုးမှုများ ရှိခဲ့ပါသည်။ Barbara Beeton မှ လက်စွဲစာအုပ်ကို ပိုမိုကောင်းမွန်အောင် ကူညီခဲ့ပါသည်။

### ကိုးကား (References)

[1] Huda Smitshuijzen Abifares, Arabic Typography, Saqi, 2001.
[2] Johannes Braams et al., The development of national LATEX styles, TUGboat 10 (1989)
[3] Yannis Haralambous, Fonts & Encodings, O'Reilly, 2007.
[4] Donald E. Knuth, The TEXbook, Addison-Wesley, 1986.
[5] Leslie Lamport, LATEX, A document preparation System, Addison-Wesley, 1986.
[6] Ken Lunde, CJKV Information Processing, O'Reilly, 2nd ed., 2009.


---

# အပိုင်း ၂ — Polyglossia (ပိုလီဂလော့စီးယား) အသုံးပြုသူလမ်းညွှန်

**မူကွဲ v2.9 | ၂၀၂၅/၁၂/၀၁**

**XƎLATEX နှင့် LuaLATEX ဖြင့် ခေတ်မီဘာသာစုံစာစီစာရိုက်**

| |
|---|
| **François Charette, Arthur Reutenauer, Udi Fogiel** |
| **Bastien Roucariès, Jürgen Spitzmüller** |

---

## ၁. နိဒါန်း (Introduction)

Polyglossia သည် XƎLATEX နှင့် LuaLATEX တို့ဖြင့် ဘာသာစုံစာစီစာရိုက်ခြင်းကို လွယ်ကူချောမွေ့စေရန် ဖန်တီးထားသော package တစ်ခုဖြစ်ပါသည်။ ၎င်းသည် babel ၏ အခြားရွေးချယ်စရာအဖြစ် အောက်ပါလုပ်ဆောင်ချက်များကို အလိုအလျောက်လုပ်ဆောင်ပေးနိုင်သည် -

၁. သင့်လျော်သော hyphenation patterns များကို တင်ခြင်း
၂. လက်ရှိဖောင့်၏ script နှင့် language tags များကို fontspec package မှတစ်ဆင့် သတ်မှတ်ခြင်း
၃. အသုံးပြုသူသတ်မှတ်ထားသော ဖောင့်သို့ ပြောင်းခြင်း
၄. လက်ရှိဘာသာစကားအလိုက် စာစီစာရိုက်ဆိုင်ရာ စည်းမျဉ်းများကို ချိန်ညှိခြင်း
၅. စာရွက်စာတမ်းစာတန်းအားလုံးကို ပြန်လည်သတ်မှတ်ခြင်း ("chapter", "figure", "bibliography" စသည်)
၆. ရက်စွဲပုံစံများကို ပြုပြင်ခြင်း (ဟီးဘရူး၊ အစ္စလာမစ်၊ ပါးရှင်းပြက္ခဒိန်များအပါအဝင်)
၇. ကိုယ်ပိုင်ဂဏန်းစနစ်ရှိသော ဘာသာစကားများအတွက် ဂဏန်းပုံစံများကို ပြုပြင်ခြင်း
၈. ညာမှဘယ်စာရေးဘာသာစကားများအတွက် ဦးတည်ချက်မှန်ကန်စေရေး (bidi package မှတစ်ဆင့်)

**လိုအပ်ချက်များ (Requirements) -**

Polyglossia ၏ လက်ရှိဗားရှင်းသည် etoolbox package မှ macro များကို အသုံးပြုထားပြီး XƎLATEX နှင့် LuaLATEX အတွက် fontspec ပေါ်တွင် မှီခိုသည်။ ညာမှဘယ်စာရေးဘာသာစကားများအတွက် bidi (XƎTEX) သို့မဟုတ် luabidi (LuaTEX) လိုအပ်ပါသည်။

---

## ၂. ဘာသာစုံစာရွက်စာတမ်းများ သတ်မှတ်ခြင်း (Setting up multilingual documents)

### ၂.၁ ဘာသာစကားများ အသက်သွင်းခြင်း (Activating languages)

```
\setdefaultlanguage{english}
\setmainlanguage{english}
\setotherlanguage{burmese}
\setotherlanguages{french,german,japanese}
```

### ၂.၂ ပံ့ပိုးထားသောဘာသာစကားများ (Supported languages)

Polyglossia သည် ဘာသာစကားများစွာကို ပံ့ပိုးထားသည် - afrikaans, arabic, armenian, belarusian, bengali, catalan, chinese, croatian, czech, danish, dutch, english (ဗားရှင်းအမျိုးမျိုး), esperanto, finnish, french (canadian, acadian, swiss), gaelic, georgian, german (austrian, swiss, spelling မူကွဲများ), greek (monotonic, polytonic, ancient), hebrew, hindi, hungarian, italian, japanese, kannada, khmer, korean, kurdish, lao, latin (classic, ecclesiastic, medieval), latvian, lithuanian, malayalam, marathi, mongolian, nko, norwegian (bokmal, nynorsk), odia, persian, piedmontese, polish, portuguese (brazilian, portuguese), punjabi, romanian, russian (spelling မူကွဲများ), sami, sanskrit (script မူကွဲများ), serbian (cyrillic, latin), slovak, slovenian, sorbian (upper, lower), spanish (mexican), swedish, syriac, tamil, telugu, thai, turkish, turkmen, ukrainian, urdu, uyghur, vietnamese နှင့် အခြားများစွာ။

### ၂.၃ Babel ဘာသာစကားအမည်များနှင့် ဆက်စပ်ပုံ (Relation to and use of Babel language names)

Polyglossia သည် babel ၏ ဘာသာစကားအမည်များကို တွဲဖက်အသုံးပြုနိုင်ရန် ဒီဇိုင်းထုတ်ထားသည်။ Table 2 (မူရင်းစာရွက်စာတမ်းတွင်) က polyglossia နှင့် babel အမည်များ၏ mapping ကို ဖော်ပြထားသည်။

### ၂.၄ IETF ဘာသာစကား tags များ အသုံးပြုခြင်း (Using IETF language tags)

BCP 47 tags များကို အသုံးပြုနိုင်သည် -

```
\setdefaultlanguage[variant=british]{english}
\setotherlanguage[variant=austrian]{german}
```

BCP 47 polyglossia mapping နမူနာများ -

| BCP-47 tag | Polyglossia အမည် | Options |
|---|---|---|
| en-GB | english | variant=british |
| en-US | english | variant=us |
| de-DE | german | variant=german, spelling=new |
| fr-CA | french | variant=canadian |
| zh-CN | chinese | variant=simplified |
| zh-TW | chinese | variant=traditional |
| my-MM | burmese | - |
| ja-JP | japanese | - |
| ar-SA | arabic | - |

### ၂.၅ ကမ္ဘာလုံးဆိုင်ရာ ရွေးချယ်စရာများ (Global options)

- `babelshorthands` - babel shorthands များကို အသက်သွင်းခြင်း
- `localmarks` - header text ကို လက်ရှိဘာသာစကားဖြင့် သတ်မှတ်ခြင်း
- `luatexrenderer` - LuaTEX အတွက် font renderer (default: Harfbuzz)

### ၂.၆ အတိုကောက်များ (Shorthands)

Polyglossia သည် babel-style shorthands များကို ပံ့ပိုးသည် -
```
\setdefaultlanguage[ babelshorthands=true ]{german}
```

---

## ၃. ဘာသာစကားပြောင်းလဲရန် ညွှန်ကြားချက်များ (Language-switching commands)

### ၃.၁ အကြံပြုထားသော ညွှန်ကြားချက်များ (Recommended commands)

```
\textenglish{This is English text}
\textgreek{Ελληνικό κείμενο}
\textlang{burmese}{မြန်မာစာသား}
```

Environment များ -
```
\begin{english}
This is an English paragraph.
\end{english}
```

```
\begin{burmese}
ဤသည်မှာ မြန်မာဘာသာစာပိုဒ်ဖြစ်ပါသည်။
\end{burmese}
```

### ၃.၂ Babel ညွှန်ကြားချက်များ (Babel commands)

```
\selectlanguage{burmese}
\foreignlanguage{burmese}{မြန်မာစာသား}
```

```
\begin{otherlanguage}{burmese}
မြန်မာဘာသာစာပိုဒ်
\end{otherlanguage}
```

### ၃.၃ အခြားညွှန်ကြားချက်များ (Other commands)

```
\selectbackgroundlanguage{english}
\resetdefaultlanguage{burmese}
\normalfontlatin
\latinalph{counter}
\latinAlph{counter}
```

### ၃.၄ Alias ညွှန်ကြားချက်များ သတ်မှတ်ခြင်း (Setting up alias commands)

```
\setlanguagealias[variant=austrian]{german}{AT}
```

---

## ၄. ဖောင့်သတ်မှတ်ခြင်း (Font setup)

```
\setmainfont{Noto Serif}
\setsansfont{Noto Sans}
\setmonofont{Noto Sans Mono}

\newfontfamily\burmesefont{Noto Sans Myanmar}[Script=Myanmar]
\newfontfamily\thaifont{Noto Sans Thai}[Script=Thai]
```

တစ်ဘာသာစကားချင်းအတွက် ဖောင့်သတ်မှတ်ခြင်း -
```
\setmainlanguage{english}
\setotherlanguage{burmese}
\newfontfamily\englishfont{Noto Serif}[Script=Latin]
\newfontfamily\burmesefont{Noto Sans Myanmar}[Script=Myanmar]
```

---

## ၅. ဝဏ္ဏခွဲခြင်းကို ပြုပြင်ခြင်း (Adapting hyphenation)

### ၅.၁ ဝဏ္ဏခွဲခြင်း ခြွင်းချက်များ (Hyphenation exceptions)

```
\pghyphenation{burmese}{example-words}
```

### ၅.၂ ဝဏ္ဏခွဲခြင်း အတိုင်းအတာများ (Hyphenation thresholds)

```
\pghyphenmins{burmese}{2}{3}
```

### ၅.၃ ဝဏ္ဏခွဲခြင်းကို ပိတ်ခြင်း (Hyphenation disabling)

```
\pghyphenation{burmese}{}
```

---

## ၆. ဘာသာစကားအလိုက် ရွေးချယ်စရာများနှင့် ညွှန်ကြားချက်များ (Language-specific options and commands)

### ၆.၁ Arabic (အာရဗီ)

```
\setotherlanguage[vocalfinal=true]{arabic}
```

### ၆.၂ French (ပြင်သစ်)

```
\setotherlanguage[variant=canadian]{french}
\AutoSpaceBeforeFDP
\NonAutoSpaceBeforeFDP
\FrenchFootnotes
```

### ၆.၃ German (ဂျာမန်)

```
\setotherlanguage[
  variant=austrian,
  spelling=new,
  babelshorthands=true
]{german}
```

### ၆.၄ Greek (ဂရိ)

```
\setotherlanguage[
  variant=polytonic,
  numerals=greek
]{greek}
\greektoday
```

### ၆.၅ Hebrew (ဟီးဘရူး)

```
\setotherlanguage[
  numerals=hebrew,
  calendar=hebrew
]{hebrew}
```

### ၆.၆ Japanese/Chinese (ဂျပန်/တရုတ်)

မှတ်ချက် - Support for Chinese and Japanese is experimental. Line breaking mechanism သည် proof of concept ဖြစ်ပါသည်။

```
\setotherlanguage[variant=simplified]{chinese}
\setotherlanguage{japanese}
```

### ၆.၇ Russian (ရုရှား)

```
\setotherlanguage[spelling=modern]{russian}
```

### ၆.၈ Sanskrit (သင်္သကရိုက်)

```
\setotherlanguage[script=Devanagari]{sanskrit}
```

---

## ၇. ဂဏန်းများနှင့် ရေတွက်ခြင်း (Numbers and numeration)

### ၇.၁ ဂဏန်းပုံစံများ (Numeral formats)

```
\localnumeral{42}
\localnumeral[arabic]{42}
\localnumeral[hebrew]{42}
```

### ၇.၂ အက္ခရာဂဏန်းများ (Alphabetic numerals)

```
\greeknumeral{42}
\hebrewnumeral{42}
\arabicnumeral{42}
```

### ၇.၃ ရက်စွဲများ (Dates)

```
\today
\greektoday
```

---

## ၈. အခြားအင်္ဂါရပ်များ (Other features)

### ၈.၁ ဘာသာစကားစစ်ဆေးခြင်း (Language querying)

```
\iflanguageloaded{burmese}{true}{false}
\languageid{bcp47}
\mainlanguageid{bcp47}
```

### ၈.၂ နောက်ထပ် အင်္ဂါရပ်များ

```
\setlanguagealias[variant=austrian]{german}{AT}
\xpg@loaded  % တင်ထားသော ဘာသာစကားအားလုံးစာရင်း
```

---

## ၉. Polyglossia ဖြင့် မြန်မာဘာသာအတွက် လက်တွေ့အသုံးချခြင်း

မြန်မာဘာသာစာရွက်စာတမ်းတစ်ခုကို Polyglossia ဖြင့် စတင်ရန် -

```
% !TEX program = xelatex
\documentclass{article}

\usepackage{polyglossia}
\setdefaultlanguage{burmese}
\setmainfont{Noto Sans Myanmar}

\begin{document}

\title{မြန်မာဘာသာစာတမ်း}
\author{စာရေးသူအမည်}
\maketitle

\section{နိဒါန်း}
ဤသည်မှာ မြန်မာဘာသာဖြင့် ရေးသားထားသော စာရွက်စာတမ်းဖြစ်ပါသည်။

\end{document}
```

Babel ဖြင့် မြန်မာဘာသာ -
```
\usepackage[burmese, provide=*]{babel}
\babelfont{rm}{Noto Sans Myanmar}
```

---

## ၁၀. ဗားရှင်းမှတ်တမ်းအကျဉ်း (Revision History Summary)

- **v2.9** (2025/12/01) - Bug fixes, CJK line breaking improvements, Korean Josa fix
- **v2.8** (2025/09/22) - CJK character spacing fixes
- **v2.7** (2025/09/11) - PDF strings fix, CJK punctuation spacing
- **v2.6** (2025/06/30) - Greek koppa option, localmarks update
- **v2.5** (2025/05/12) - Latin name changes, bug fixes
- **v2.4** (2025/01/31) - Bengali fix, language testing fix
- **v2.3** (2024/09/23) - Japanese/Chinese line breaking
- **v2.2** (2024/07/15) - Performance improvements, font association
- **v2.1** (2024/03/07) - Bug fixes
- **v2.0** (2024/02/17) - Major rewrite, latex3, German gender shorthands
- **v1.0** (2008/07/13) - Initial release on CTAN

---

## ၁၁. ကျေးဇူးတင်လွှာ (Acknowledgements)

Polyglossia သည် အခြားသူများ၏ ပံ့ပိုးမှုများကို ပြန်လည်အသုံးပြုထားသော package တစ်ခုဖြစ်ပါသည်။ အထူးကျေးဇူးတင်ရှိပါသည် -

- Johannes Braams နှင့် babel package အတွက် ပံ့ပိုးသူအားလုံး
- Will Robertson (fontspec)
- Vafa Khalighi (xepersian နှင့် bidi)
- Mojca Miklavec နှင့် Arthur Reutenauer (hyph-utf8)
- Jonathan Kew (XƎTEX တီထွင်သူ)

ဘာသာစကားအလိုက် ပံ့ပိုးသူများ - Yves Codet (Sanskrit), Zdeněk Wagner (Hindi), Mikhail Oren (Hebrew), Khaled Hosny (Arabic), Kevin Godby (Asturian, Lithuanian, Occitan, Bengali, Malayalam, Marathi, Tamil, Telugu) နှင့် အခြားများစွာ။

---

## နိဂုံး

Babel နှင့် Polyglossia နှစ်ခုစလုံးသည် LaTeX တွင် ဘာသာစုံစာစီစာရိုက်အတွက် အစွမ်းထက်သော tools များဖြစ်ပါသည် -

- **Babel** သည် pdfTeX, LuaTeX, XeTeX အားလုံးကို ပံ့ပိုးပြီး ဘာသာစကားများစွာအတွက် ရင့်ကျက်သော ပံ့ပိုးမှုရှိသည်
- **Polyglossia** သည် XeLaTeX နှင့် LuaLaTeX အတွက် အထူးဒီဇိုင်းထုတ်ထားပြီး ပိုမိုသန့်ရှင်းပေါ့ပါးသော ဒီဇိုင်းရှိသည်

မြန်မာဘာသာအတွက် နှစ်ခုစလုံးကို အသုံးပြုနိုင်ပြီး၊ Unicode Myanmar ဖောင့်များ (Noto Sans Myanmar, Padauk, Myanmar Text စသည်) ကို ထောက်ပံ့ပေးနိုင်ပါသည်။
