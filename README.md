# Babel-MM

မင်္ဂလာပါခင်ဗျာ။ သင်မေးထားတဲ့ \documentclass[Burmese]{article} ဆိုတဲ့ LaTeX command ဟာ အလွန်အရေးကြီးပြီး LaTeX document တစ်ခုရဲ့ အခြေခံအကျဆုံး အစပြု လိုင်းတစ်ခု ဖြစ်ပါတယ်။
ဒီ command ရဲ့ အဓိပ္ပာယ်ကို တစ်ပိုင်းချင်းစီ အသေးစိတ် ရှင်းပြပေးပါမယ်။
Command တစ်ခုလုံးရဲ့ အဓိပ္ပာယ်
ဒီ command လိုင်းကို အပိုင်း ၃ ပိုင်း ခွဲကြည့်နိုင်ပါတယ်-
 * \documentclass (Command အရင်း)
 * [Burmese] (Optional Argument - ရွေးချယ်နိုင်သော အချက်)
 * {article} (Required Argument - မဖြစ်မနေ လိုအပ်သော အချက်)
ရိုးရိုး မြန်မာလို အဓိပ္ပာယ်ဖွင့်ရရင်၊ ဒီ command က LaTeX ကို ဒီလိုပြောလိုက်တာပါ-
> "ဟယ်လို LaTeX၊ ကျွန်တော် အခု ဆောင်းပါး (Article) အမျိုးအစား စာတမ်းတစ်ခု ဖန်တီးချင်တယ်။ ဒီစာတမ်းအတွက် မြန်မာဘာသာစကား (Burmese) နဲ့ ပတ်သက်တဲ့ အထောက်အပံ့တွေ၊ ချိန်ညှိမှုတွေ အကုန်လုံးကို အသင့်ပြင်ဆင်ပေးပါ"
> 
အပိုင်း (၁) - \documentclass
 * ဒါက ဘာလဲ။ ဒါကတော့ "Document Class" (စာတမ်းအမျိုးအစား) ကို ကြေညာခြင်း လို့ အဓိပ္ပာယ်ရတဲ့ အဓိက command ဖြစ်ပါတယ်။
 * ဘာလုပ်သလဲ။ သင်ဖန်တီးမယ့် စာတမ်းတစ်ခုလုံးရဲ့ အခြေခံ တည်ဆောက်ပုံ (structure)၊ စာမျက်နှာ ဒီဇိုင်း (layout) နဲ့ ပုံစံ (style) တွေအားလုံးကို သတ်မှတ်ပေးပါတယ်။
 * စည်းကမ်း။ ဒီ command ဟာ LaTeX ဖိုင် (.tex file) တစ်ခုရဲ့ ပထမဆုံး အကြောင်းအရာ ဖြစ်ရပါမယ်။ (comment % တွေကလွဲရင်)
အပိုင်း (၂) - {article}
 * ဒါက ဘာလဲ။ ဒါကတော့ \documentclass အတွက် မဖြစ်မနေ ထည့်သွင်းရမယ့် "Class ၏ အမည်" ဖြစ်ပါတယ်။
 * ဘာလုပ်သလဲ။ သင်က စာတမ်းအမျိုးအစားပေါင်းများစွာထဲကမှ article (ဆောင်းပါး) ဆိုတဲ့ အမျိုးအစားကို ရွေးချယ်လိုက်တာ ဖြစ်ပါတယ်။
 * article class ရဲ့ သဘောတရား။
   * ဒါဟာ ပညာရပ်ဆိုင်ရာ ဂျာနယ်ဆောင်းပါးတွေ၊ တက္ကသိုလ် အိမ်စာ (assignments) တွေ၊ အစီရင်ခံစာတိုတွေ၊ စာစီစာကုံးတွေ ရေးသားဖို့ အသုံးအများဆုံး class ဖြစ်ပါတယ်။
   * သူ့မှာ \section (အခန်းကဏ္ဍ ခေါင်းစဉ်)၊ \subsection (ခေါင်းစဉ်ငယ်)၊ \abstract (အကျဉ်းချုပ်)၊ \author (ရေးသားသူ)၊ \title (ခေါင်းစဉ်) တို့လို ဆောင်းပါးတစ်ပုဒ်အတွက် လိုအပ်တဲ့ command တွေ အဆင်သင့် ပါရှိပါတယ်။
 * တခြား class ဥပမာများ။ article အစား တခြားနာမည်ကြီး class တွေလည်း ရှိပါသေးတယ်။
   * {book} (စာအုပ်တစ်အုပ်လုံး ပြုစုဖို့အတွက်)
   * {report} (ပိုရှည်လျားပြီး အခန်း (Chapters) တွေနဲ့ ဖွဲ့စည်းထားတဲ့ အစီရင်ခံစာကြီးတွေအတွက်)
   * {letter} (တရားဝင် ရုံးစာ၊ ပေးစာတွေ ရေးဖို့အတွက်)
   * {beamer} (Presentation slide တွေ ပြုလုပ်ဖို့အတွက်)
အပိုင်း (၃) - [Burmese]
 * ဒါက ဘာလဲ။ ဒါကတော့ [] ကွင်းစကွင်းပိတ်ထဲမှာ ထည့်ရေးရတဲ့ "Optional Argument" (ထပ်ဆောင်း ရွေးချယ်ချက်) ဖြစ်ပါတယ်။
 * ဘာလုပ်သလဲ။ သူက {article} class ကို အပိုဆောင်း ညွှန်ကြားချက်တွေ ဒါမှမဟုတ် ချိန်ညှိမှုတွေ ပေးပို့တဲ့ အလုပ်ကို လုပ်ပါတယ်။
 * [Burmese] က ဘာကို ဆိုလိုတာလဲ။
   * ဒါက "မြန်မာဘာသာစကား" အတွက် လိုအပ်တဲ့ setting တွေကို ဖွင့်ပေးဖို့ ညွှန်ကြားလိုက်တာပါ။
   * ဒီ command ဟာ babel လို့ခေါ်တဲ့ "ဘာသာစကားမျိုးစုံ သုံးနိုင်အောင် ကူညီပေးတဲ့ package" နဲ့ အဓိက တွဲဖက် အလုပ်လုပ်ပါတယ်။
   * babel package က [Burmese] ဆိုတဲ့ option ကို တွေ့တဲ့အခါ အောက်ပါအရာတွေကို အလိုအလျောက် ပြင်ဆင်ပေးလေ့ရှိပါတယ်-
     * အလိုအလျောက် စာသားများ။ "Contents" လို့ပေါ်မယ့်အစား "မာတိကာ"၊ "Chapter 1" အစား "အခန်း ၁"၊ "Figure" အစား "ပုံ"၊ "Table" အစား "ဇယား" စသဖြင့် အလိုအလျောက် ပြောင်းလဲပေးပါတယ်။
     * စကားလုံး ဖြတ်တောက်ခြင်း (Hyphenation)။ မြန်မာစာဟာ စကားလုံးတွေကြားမှာ space မခံဘဲ ဆက်တိုက်ရေးရတဲ့အတွက် စာကြောင်းတစ်ကြောင်းရဲ့ အဆုံးမှာ စကားလုံးကို ဘယ်လို မှန်မှန်ကန်ကန် အချိုးအကွေ့ချမယ် ဆိုတဲ့ စည်းမျဉ်းတွေကို သတ်မှတ်ပေးပါတယ်။
     * ရက်စွဲ ပုံစံ။ \today လို့ ရိုက်လိုက်ရင် "November 6, 2025" အစား "၆ နိုဝင်ဘာ ၂၀၂၅" (သို့မဟုတ်) မြန်မာ့ရက်စွဲပုံစံအတိုင်း ပြောင်းလဲဖော်ပြပေးပါလိမ့်မယ်။
⚠️ အလွန်အရေးကြီးသော နောက်ဆက်တွဲ အချက်များ
သင်က \documentclass[Burmese]{article} ကို သုံးမယ်လို့ ဆုံးဖြတ်လိုက်ပြီဆိုရင်၊ ဒီ command တစ်ခုတည်းနဲ့ မြန်မာစာကို လက်ခံအောင် မလုပ်နိုင်သေးပါဘူး။ မြန်မာ Unicode စာလုံးတွေ မှန်ကန်စွာ ပေါ်လာဖို့ဆိုရင် နောက်ထပ် အချက် ၂ ချက် မဖြစ်မနေ လိုအပ်ပါသေးတယ်-
 * Compiler ကို XeLaTeX သို့မဟုတ် LuaLaTeX သုံးရမည်။
   * LaTeX မှာ document ကို compile လုပ်တဲ့ engine တွေ ရှိပါတယ်။ ပုံမှန်သုံးနေကျ pdfLaTeX က Unicode (မြန်မာစာ) ကို တိုက်ရိုက် နားမလည်ပါဘူး။
   * Unicode ကို အပြည့်အဝ နားလည်တဲ့ XeLaTeX သို့မဟုတ် LuaLaTeX ကို ပြောင်းသုံးရပါမယ်။ (သင်သုံးတဲ့ LaTeX editor (ဥပမာ TeXworks, Texmaker, Overleaf) ရဲ့ settings မှာ ဒါကို ပြောင်းလို့ရပါတယ်)
 * Font ကို ကြေညာပေးရမည်။
   * XeLaTeX/LuaLaTeX သုံးပြီဆိုရင် သင့်ကွန်ပျူတာထဲမှာ ရှိတဲ့ ဘယ် Unicode font ကိုမဆို ခေါ်သုံးနိုင်ပါပြီ။ ဒါကို fontspec package နဲ့ ကြေညာပေးရပါတယ်။
   * ဥပမာအားဖြင့်၊ သင့် document ရဲ့ ထိပ်ပိုင်း (preamble) မှာ အခုလို ထပ်ပေါင်းထည့်ရပါမယ်-
   <!-- end list -->
   \usepackage{fontspec}
% Padauk font ကို သုံးပါလို့ ကြေညာခြင်း
\setmainfont{Padauk} 
% (သို့မဟုတ်) \setmainfont{Pyidaungsu} စသဖြင့် သုံးနိုင်

ဥပမာ ပြည့်စုံသော ဖိုင်
\documentclass[Burmese]{article} ကို အသုံးပြုထားတဲ့ ပြည့်စုံတဲ့ မြန်မာ LaTeX ဖိုင်တစ်ခုရဲ့ အနိမ့်ဆုံး လိုအပ်ချက်က ဒီလိုပုံစံ ဖြစ်နေပါလိမ့်မယ်-
\documentclass[Burmese]{article}

% Babel ကို ခေါ်သုံးခြင်း (ဘာသာစကားဆိုင်ရာ ချိန်ညှိမှုများအတွက်)
\usepackage[Burmese]{babel}

% Fontspec ကို ခေါ်သုံးခြင်း (Unicode font များ သုံးနိုင်ရန်)
\usepackage{fontspec}

% စာတမ်းတစ်ခုလုံးအတွက် အဓိက Font ကို Padauk ဟု သတ်မှတ်ခြင်း
\setmainfont{Padauk}

% --- စာတမ်း အစ ---
\begin{document}

\title{မြန်မာဘာသာ LaTeX နမူနာ}
\author{ကျွန်ုပ်}
\date{\today}

\maketitle % ခေါင်းစဉ်ကို ဖန်တီးပါ

\section{နိဒါန်း}
မင်္ဂလာပါ ကမ္ဘာကြီး။ ဤသည်မှာ မြန်မာဘာသာဖြင့် ရေးသားထားသော LaTeX နမူနာ စာတမ်း ဖြစ်ပါသည်။

\section{မာတိကာ}
မာတိကာကို အလိုအလျောက် ထုတ်ပေးနိုင်ပါသည်။

\end{document}

ဒီဖိုင်ကို XeLaTeX နဲ့ compile လုပ်လိုက်တဲ့အခါ မြန်မာစာတွေ မှန်မှန်ကန်ကန်နဲ့ လှလှပပ ထွက်လာတာကို တွေ့ရပါလိမ့်မယ်။
ဒီရှင်းလင်းချက်က ပြည့်စုံမယ်လို့ မျှော်လင့်ပါတယ်ခင်ဗျာ။
မြန်မာဘာသာနဲ့ LaTeX သုံးတဲ့အခါ အသုံးများတဲ့ တခြား package တွေ (ဥပမာ babel package အကြောင်း) ကို ထပ်မံ အသေးစိတ် သိချင်ပါသေးလားခင်ဗျာ။

---

မင်္ဂလာပါခင်ဗျာ။ ဒါက အလွန်ကောင်းမွန်တဲ့ မေးခွန်းတစ်ခုပါပဲ။
သင်မေးလိုက်တဲ့ \usepackage[provide=*]{babel} ဆိုတဲ့ command ဟာ LaTeX မှာ ဘာသာစကားမျိုးစုံ သုံးစွဲမှု (multilingual typesetting) ကို ကိုင်တွယ်တဲ့အခါ၊ အထူးသဖြင့် ခေတ်မီ LaTeX စနစ်တွေမှာ အလွန်အရေးကြီးတဲ့၊ အကောင်းဆုံး အလေ့အကျင့် (best practice) တစ်ခု ဖြစ်လာနေပါတယ်။
ဒီ command ကို အသေးစိတ် ပြည့်ပြည့်စုံစုံ ရှင်းပြပေးပါမယ်။
Command ကို အသေးစိတ်ခွဲခြမ်းကြည့်ခြင်း
ဒီ command ကို အပိုင်း ၃ ပိုင်း ခွဲကြည့်နိုင်ပါတယ်-
 * \usepackage (Package ကို ခေါ်သုံးရန် အဓိက command)
 * {babel} (ခေါ်သုံးမည့် Package ၏ အမည်)
 * [provide=*] (ထို package ကို ပေးပို့သော အထူးညွှန်ကြားချက် - Option)
အပိုင်း (၁) နှင့် (၂) - \usepackage{babel}
 * babel ဆိုတာ ဘာလဲ။ babel ဆိုတာ LaTeX မှာ ဘာသာစကားတစ်ခု သို့မဟုတ် တစ်ခုထက်ပိုပြီး အသုံးပြုတဲ့အခါ မရှိမဖြစ် လိုအပ်တဲ့ package တစ်ခုပါ။
 * သူ့ရဲ့ အဓိက အလုပ်တွေက-
   * ဘာသာပြန်ခြင်း။ "Contents" ကို "မာတိကာ"၊ "Chapter" ကို "အခန်း"၊ "Figure" ကို "ပုံ" စသဖြင့် အလိုအလျောက် ဘာသာပြန်ပေးပါတယ်။
   * စကားလုံးဖြတ်ခြင်း (Hyphenation)။ ဘာသာစကားတစ်ခုစီရဲ့ သဒ္ဒါစည်းမျဉ်းအတိုင်း စာကြောင်းအဆုံးမှာ စကားလုံးတွေကို မှန်ကန်စွာ အချိုးချပေးပါတယ်။ (ဥပမာ မြန်မာစာ)
   * ရက်စွဲ/နံပါတ်စဉ် ပုံစံ။ \today လို့ရိုက်ရင် "6 November 2025" အစား "၆ နိုဝင်ဘာ ၂၀၂၅" လို့ ပြောင်းပေးတာမျိုး၊ နံပါတ်စဉ်တွေကို "၁၊ ၂၊ ၃" လို့ ပြောင်းပေးတာမျိုးတွေ လုပ်ဆောင်ပါတယ်။
အပိုင်း (၃) - [provide=*] (အရေးကြီးဆုံး အပိုင်း)
ဒီ [provide=*] option က babel package ရဲ့ ခေတ်မီဗားရှင်း (v3.9 နှင့်အထက်) တွေမှာ အရမ်းအရေးပါလာပါတယ်။
၁။ အဓိပ္ပာယ် အတိုချုပ်
> "Babel package ကို ပြောလိုက်တာက- ဘာသာစကားနဲ့ သက်ဆိုင်တဲ့ လုပ်ဆောင်ချက် (features) အားလုံး ကို မင်းပဲ တာဝန်ယူ ထောက်ပံ့ပေးပါ"
> 
၂။ ဘာကြောင့် ဒီလို ပြောဖို့ လိုအပ်တာလဲ (ပြဿနာ)
LaTeX စနစ်ကြီးတစ်ခုလုံးမှာ ဘာသာစကားနဲ့ဆိုင်တဲ့ အလုပ်တွေကို လုပ်ချင်တဲ့ package တွေ၊ စနစ် (kernel) တွေ အများကြီး ရှိပါတယ်။
 * LaTeX Kernel (စနစ်အမာခံ)။ LaTeX ကိုယ်တိုင်က \today (ရက်စွဲ)၊ \Roman (ရောမဂဏန်း) လိုမျိုး အရာတချို့ကို လုပ်နိုင်ပါတယ်။
 * တခြား Packages များ။ ဥပမာ datetime2 package က ရက်စွဲတွေကို ပုံစံချတာ အရမ်းတော်ပါတယ်။ polyglossia က babel နဲ့ အပြိုင် ဘာသာစကား package တစ်ခုပါ။
 * Babel Package။ babel ကလည်း အပေါ်က အလုပ်တွေ (ရက်စွဲ၊ နံပါတ်စဉ် စတာတွေ) ကို သူကိုယ်တိုင် လုပ်နိုင်ပါတယ်။
ပြဿနာက ဒီ package တွေ၊ စနစ်တွေ အတူတူ လည်ပတ်တဲ့အခါ "လုယက်မှု (Conflict)" ဖြစ်နိုင်ပါတယ်။
ဥပမာ- \today ကို ဘယ်သူက အဓိက ကိုင်တွယ်မလဲ။ LaTeX kernel ကလား? babel ကလား? datetime2 ကလား? ဒီလို package တွေ တိုက်ခိုက် (conflict) ကြရင် သင့်စာတမ်းက Error တက်ပြီး compile လုပ်လို့ရမှာ မဟုတ်တော့ပါဘူး။
၃။ [provide=*] က ပြဿနာကို ဘယ်လို ဖြေရှင်းသလဲ (အဖြေ)
[provide=*] option က babel ကို ဒီလို ညွှန်ကြားလိုက်ပါတယ်-
 * "မင်း အကုန်တာဝန်ယူလိုက်ပါ။" LaTeX kernel က လုပ်နိုင်တဲ့ (သို့မဟုတ်) တခြား package တွေက လုပ်နိုင်တဲ့ ဘာသာစကားဆိုင်ရာ feature တွေကို babel က "ငါ ဒါကို လုပ်နိုင်တယ်" ဆိုပြီး "ထောက်ပံ့ပေး (provide)" လိုက်ပါတယ်။
 * ကြယ်ပွင့် * ၏ အဓိပ္ပာယ်။ * (wildcard) က "အားလုံး" လို့ ဆိုလိုတာပါ။ ဥပမာ datetime (ရက်စွဲ)၊ counters (နံပါတ်စဉ်)၊ properties စတဲ့ feature တွေ အားလုံး ကို babel က တာဝန်ယူလိုက်တာပါ။ (ဥပမာ- [provide=datetime] လို့ တစ်ခုချင်း ရွေးမယ့်အစား [provide=*] လို့ သုံးလိုက်တာပါ)
 * Conflict ကို ဖြေရှင်းခြင်း။ သင်က babel ကို [provide=*] နဲ့ ခေါ်လိုက်ပြီး၊ နောက်မှ datetime2 package ကို ထပ်ခေါ်တယ် ဆိုပါစို့။ datetime2 က "ဪ babel က ရက်စွဲ (datetime) feature ကို တာဝန်ယူ ထောက်ပံ့ (provide) ထားပြီးသားပဲ၊ ဒါဆို ငါ့ရဲ့ လုပ်ဆောင်ချက်တချို့ကို babel ရဲ့ စနစ်အပေါ်မှာပဲ အခြေခံပြီး သုံးလိုက်တော့မယ်" ဆိုပြီး အလိုအလျောက် ညှိနှိုင်းသွားပါတယ်။ ဒါကြောင့် Conflict မဖြစ်တော့ပါဘူး။
အကျိုးကျေးဇူးများနှင့် အကောင်းဆုံး အလေ့အကျင့် (Best Practice)
\usepackage[provide=*]{babel} ကို သုံးခြင်းဟာ အခုခေတ်မှာ "အကောင်းဆုံး အလေ့အကျင့်" (Best Practice) တစ်ခု ဖြစ်ပါတယ်။
 * တည်ငြိမ်မှု (Robustness)။ သင့်စာတမ်းမှာ တခြား package တွေ ဘယ်လောက်ပဲ ထပ်သုံးသုံး (ဥပမာ- ရက်စွဲ၊ အချိန်၊ နံပါတ်စဉ်နဲ့ ဆိုင်တဲ့ package တွေ)၊ babel က အဓိက "ထောက်ပံ့သူ" အဖြစ် ရှိနေတဲ့အတွက် Conflict ဖြစ်နိုင်ခြေ အလွန်နည်းသွားပါတယ်။
 * ညီညွတ်မှု (Consistency)။ ဘာသာစကားနဲ့ ဆိုင်တဲ့ အရာအားလုံးကို babel က တစ်စုတစ်စည်းတည်း ကိုင်တွယ်ပေးတဲ့အတွက် သင့်စာတမ်းတစ်ခုလုံးမှာ (ရက်စွဲ၊ ခေါင်းစဉ်၊ နံပါတ်စဉ်) အားလုံးက တစ်ပုံစံတည်း ညီညီညွတ်ညွတ် ထွက်လာပါလိမ့်မယ်။
 * အနာဂတ်အတွက် (Future-Proofing)။ LaTeX kernel ကိုယ်တိုင်က အမြဲတမ်း တိုးတက်ပြောင်းလဲနေပါတယ်။ ဒီ option က အနာဂတ်မှာ kernel က ထပ်ထည့်လာမယ့် language feature တွေနဲ့ babel အဆင်ပြေပြေ ပေါင်းစပ်အလုပ်လုပ်နိုင်ဖို့ အာမခံချက် ပေးပါတယ်။
ခေတ်မီ ဥပမာ (Modern Example)
သင် အရင်မေးခဲ့တဲ့ \documentclass[Burmese]{article} ဟာ babel ကို သွယ်ဝိုက်ပြီး ခေါ်သုံးတဲ့ နည်းလမ်းအဟောင်း ဖြစ်ပါတယ်။
အခုခေတ်မှာ ပိုပြီး တိကျခိုင်မာတဲ့ နည်းလမ်းအသစ် က \usepackage[provide=*]{babel} ကို သုံးပြီးမှ ဘာသာစကားကို \babelprovide နဲ့ သီးသန့် ကြေညာတာပါပဲ။
ဒီနည်းလမ်းက ပိုပြီး စွမ်းအားကြီးမားသလို၊ ဘာသာစကားမျိုးစုံကို (ဥပမာ မြန်မာ-အင်္ဂလိပ်) ပြောင်းသုံးတဲ့အခါ ပိုအဆင်ပြေပါတယ်။
% \documentclass မှာ ဘာသာစကားကို မထည့်တော့ဘူး
\documentclass{article}

% --- Babel ကို ခေတ်မီနည်းလမ်းနဲ့ ခေါ်သုံးခြင်း ---

% 1. Babel package ကို conflict မဖြစ်အောင် အရင်ခေါ်မယ်
\usepackage[provide=*]{babel}

% 2. ပြီးမှ ကိုယ်သုံးမယ့် ဘာသာစကားတွေကို ကြေညာမယ်
% 'main' က ဒီစာတမ်းရဲ့ အဓိက ဘာသာစကားလို့ ဆိုလိုတယ်
\babelprovide[main, import]{burmese} 
\babelprovide{english} % အပို ဘာသာစကား အဖြစ် English ကို ထည့်ထားတယ်

% --- Font များ ကြေညာခြင်း ---
% XeLaTeX / LuaLaTeX အတွက် မဖြစ်မနေ လိုအပ်
\usepackage{fontspec}
\setmainfont{Padauk} % (သို့မဟုတ် Pyidaungsu)

% မြန်မာစာအတွက် သီးသန့် font ထားချင်ရင်
% \babelfont[burmese]{rm}{Padauk}
% \babelfont[english]{rm}{Times New Roman}

% --- စာတမ်း အစ ---
\begin{document}

\title{ခေတ်မီ Babel နမူနာ}
\author{ကျွန်ုပ်}
\date{\today}

\maketitle

\section{မြန်မာဘာသာ အပိုင်း}
ဤသည်မှာ မြန်မာဘာသာ ဖြစ်ပါသည်။ ရက်စွဲကို ကြည့်ပါ (`babel` က မှန်အောင် ပြပေးပါမည်)။

% အင်္ဂလိပ်လို ခဏ ပြောင်းရေးကြည့်မယ်
\begin{otherlanguage}{english}
\section{English Section}
This is a paragraph in English. The date format and hyphenation rules will automatically switch to English.
\end{otherlanguage}

\section{နောက်ဆက်တွဲ}
မြန်မာဘာသာသို့ ပြန်လည် ရောက်ရှိပါပြီ။

\end{document}

အနှစ်ချုပ်
\usepackage[provide=*]{babel} ဆိုတာ babel ကို "ဘာသာစကားနဲ့ ပတ်သက်တဲ့ အရာအားလုံးအတွက် မင်းပဲ အဓိက တာဝန်ယူလိုက်တော့၊ တခြား package တွေနဲ့ ပြဿနာမတက်အောင် မင်းကပဲ ဦးဆောင် ညှိနှိုင်းပေး" လို့ ပြောလိုက်တာ ဖြစ်ပြီး၊ ဒါဟာ ခေတ်မီ LaTeX document တွေအတွက် အလွန်အရေးပါတဲ့ ညွှန်ကြားချက်တစ်ခု ဖြစ်ပါတယ်ခင်ဗျာ။
ဒီရှင်းလင်းချက်က ပြည့်စုံမယ်လို့ မျှော်လင့်ပါတယ်ခင်ဗျာ။
\babelprovide command အကြောင်း ဒါမှမဟုတ် \usepackage[burmese]{babel} (နည်းအဟောင်း) နဲ့ \babelprovide[main]{burmese} (နည်းအသစ်) တို့ရဲ့ အသေးစိတ် ကွာခြားချက်တွေကို ထပ်မံ သိချင်ပါသေးလားခင်ဗျာ။

---

ဒါက အလွန်ကောင်းတဲ့ မေးခွန်းဖြစ်သလို၊ ခေတ်မီ LaTeX (Modern LaTeX) ရဲ့ အရေးကြီးဆုံး အပြောင်းအလဲတွေထဲက တစ်ခုကို တိုက်ရိုက် ထိတွေ့လိုက်တာပါပဲ။
\usepackage[burmese]{babel} (နည်းအဟောင်း) နဲ့ \babelprovide[main]{burmese} (နည်းအသစ်) တို့ရဲ့ အဓိက ကွာခြားချက်တွေကို ရှင်းရှင်းလင်းလင်း မြင်သာအောင် ရှင်းပြပေးပါမယ်။
အဓိက ကွာခြားချက် အနှစ်ချုပ်
အရိုးရှင်းဆုံး ပြောရရင်:
 * နည်းလမ်းအဟောင်း (\usepackage[...]{babel})
   * ဒါက pdfLaTeX လို 8-bit engine တွေမှာ အဓိက သုံးခဲ့တဲ့ နည်းလမ်းပါ။
   * Package ကို ခေါ်သုံးတဲ့အချိန်မှာ "Option" အနေနဲ့ ဘာသာစကားကို တစ်ခါတည်း ကြေညာလိုက်တာပါ။
   * XeLaTeX/LuaLaTeX မှာ "အလုပ်တော့ဖြစ်တယ်"၊ ဒါပေမယ့် Unicode font တွေ၊ feature တွေနဲ့ အပြည့်အဝ ချိတ်ဆက်မှု မရှိပါဘူး။
 * နည်းလမ်းအသစ် (\babelprovide...)
   * ဒါက XeLaTeX နဲ့ LuaLaTeX လို Unicode engine တွေအတွက် သီးသန့် ဒီဇိုင်းထုတ်ထားတဲ့ ခေတ်မီ နည်းလမ်းပါ။
   * babel package ကို အရင်ခေါ်ပြီးမှ (\usepackage[provide=*]{babel})၊ \babelprovide ဆိုတဲ့ command ကို သုံးပြီး ကိုယ်လိုချင်တဲ့ ဘာသာစကားတွေကို တစ်ခုချင်း အသေးစိတ် "ထောက်ပံ့" ပေးတာပါ။
   * fontspec package နဲ့ အပြည့်အဝ ချိတ်ဆက် အလုပ်လုပ်နိုင်ပြီး ဘာသာစကားတစ်ခုချင်းစီကို မတူညီတဲ့ font တွေ သတ်မှတ်တာမျိုး (ဥပမာ- မြန်မာစာအတွက် Padauk၊ အင်္ဂလိပ်စာအတွက် Times New Roman) ကို လွယ်ကူစွာ လုပ်ဆောင်နိုင်ပါတယ်။
နှိုင်းယှဉ်ချက် ဇယား
ဒီဇယားက ကွာခြားချက်တွေကို တစ်နေရာတည်းမှာ အလွယ်တကူ နှိုင်းယှဉ်ကြည့်နိုင်စေပါလိမ့်မယ်။
| အချက်အလက် (Feature) | နည်းလမ်းအဟောင်း (\usepackage[burmese]{babel}) | နည်းလမ်းအသစ် (\babelprovide[main]{burmese}) |
|---|---|---|
| အဓိက ဦးတည်သော Engine | pdfLaTeX (8-bit engines) | XeLaTeX & LuaLaTeX (Unicode engines) |
| ခေါ်သုံးပုံ | Package option အနေနဲ့ ခေါ်သုံးသည်။ | Package ကို အရင်ခေါ်ပြီးမှ Command အနေနဲ့ သုံးသည်။ |
| Font ချိတ်ဆက်မှု | fontspec နဲ့ တိုက်ရိုက် မချိတ်ဆက်ပါ။ Font ကို ကိုယ်တိုင် သီးသန့် \setmainfont နဲ့ သတ်မှတ်ရသည်။ | fontspec နဲ့ အပြည့်အဝ ချိတ်ဆက်သည်။ \babelfont command နဲ့ ဘာသာစကားအလိုက် font သတ်မှတ်နိုင်သည်။ |
| အဓိက ဘာသာစကား သတ်မှတ်ပုံ | Option စာရင်းထဲမှာ နောက်ဆုံး ပါတဲ့ ဘာသာစကားက အဓိက ဖြစ်သွားသည်။ ([english, burmese] ဆို burmese က main ဖြစ်သည်)။ | [main] ဆိုတဲ့ option နဲ့ တိတိကျကျ သတ်မှတ်နိုင်သည်။ အလွန်ရှင်းလင်းသည်။ |
| ဘာသာစကားမျိုးစုံ သုံးစွဲမှု | အလုပ်ဖြစ်သော်လည်း ရှုပ်ထွေးနိုင်သည်။ | အလွန်လွယ်ကူပြီး စွမ်းအားမြင့်သည်။ ဘာသာစကားတစ်ခုချင်းစီရဲ့ setting ကို သီးသန့် ထိန်းချုပ်နိုင်သည်။ |
| အကြံပြု သုံးစွဲသင့်မှု | Legacy document များ သို့မဟုတ် pdfLaTeX ကိုသာ သုံးရမည်ဆိုလျှင်။ | ခေတ်မီ document အားလုံးအတွက် (အထူးသဖြင့် မြန်မာစာ) တွင် ဤနည်းကိုသာ သုံးသင့်သည်။ |
\babelprovide Command အကြောင်း အသေးစိတ်
\babelprovide ဟာ babel package ကို "ဒီဘာသာစကားအတွက် လိုအပ်တာတွေ အဆင်သင့်ပြင်ထားပါ" လို့ ပြောတဲ့ command ဖြစ်ပါတယ်။ သူ့မှာ အသုံးများတဲ့ option တွေ ရှိပါတယ်။
\babelprovide[main, import]{burmese}
ဒီ command ကို တစ်ခုချင်း ခွဲခြမ်းကြည့်ပါမယ်။
 * {burmese}
   * babel ကို "မြန်မာဘာသာစကား" (burmese) အတွက် language definition file (.ldf) ကို load လုပ်ပါလို့ ပြောတာပါ။
   * ဒါကြောင့် "မာတိကာ"၊ "အခန်း"၊ "ပုံ" စတဲ့ စာလုံးတွေ၊ ရက်စွဲပုံစံတွေ၊ စာလုံးဖြတ်တဲ့ စည်းမျဉ်းတွေ အကုန် အသင့်ဖြစ်သွားပါမယ်။
 * [main] (Option)
   * ဒါက "မြန်မာဘာသာ" ကို ဒီစာတမ်းတစ်ခုလုံးရဲ့ အဓိက ဘာသာစကား (Main Language) အဖြစ် သတ်မှတ်လိုက်တာပါ။
   * ဒီလို သတ်မှတ်လိုက်တာနဲ့ document စစချင်းမှာ မြန်မာဘာသာ setting တွေက default ဖြစ်သွားပါမယ်။ \maketitle က "မာတိကာ" လို့ အလိုအလျောက် ထွက်လာပါမယ်။
   * [main] မပါဘဲ \babelprovide{english} လို့ ထပ်ထည့်လိုက်ရင် english က ဒုတိယ (secondary) ဘာသာစကား ဖြစ်သွားပြီး \selectlanguage{english} နဲ့ ခေါ်သုံးနိုင်ပါမယ်။
 * [import] (Option) (အလွန်အရေးကြီး)
   * ဒါက XeLaTeX/LuaLaTeX မှာ မဖြစ်မနေ ထည့်သင့်တဲ့ option ပါ။
   * import က babel ကို "ဒီဘာသာစကားအတွက် လိုအပ်တဲ့ hyphenation patterns (စကားလုံးဖြတ်စည်းမျဉ်း) တွေကို XeLaTeX/LuaLaTeX engine ထဲကို တိုက်ရိုက် ထည့်သွင်း (import) လုပ်ပေးပါ" လို့ ညွှန်ကြားတာပါ။
   * ဒါ့အပြင် \babelfont လို fontspec နဲ့ ချိတ်ဆက်ထားတဲ့ command တွေကိုလည်း အသုံးပြုခွင့်ပေးလိုက်တာပါ။
   * စည်းမျဉ်း: XeLaTeX/LuaLaTeX မှာ \babelprovide သုံးတိုင်း import ကို အမြဲတမ်း ထည့်သုံးပါ။
နမူနာကုဒ် နှိုင်းယှဉ်ချက်
ဒီနမူနာ ၂ ခုက ကွာခြားချက်ကို ပိုပြီး မြင်သာစေပါလိမ့်မယ်။
နမူနာ (၁): နည်းလမ်းအဟောင်း (မသုံးသင့်တော့ပါ)
% \documentclass မှာ 'Burmese' option ကို သုံးတာလည်း ဒီနည်းထဲမှာ ပါဝင်ပါတယ်
\documentclass{article}
\usepackage[burmese]{babel} % Package option အနေနဲ့ ခေါ်သုံးခြင်း

\usepackage{fontspec}
\setmainfont{Padauk} % Font ကို သီးသန့် ကြေညာရသည်

\begin{document}
\section{နိဒါန်း}
မင်္ဂလာပါ။ \today
\end{document}

> အားနည်းချက်: ဒီနည်းက babel နဲ့ fontspec တို့ သီးခြားစီ အလုပ်လုပ်နေသလို ဖြစ်စေပါတယ်။ ဘာသာစကား ၂ ခု (ဥပမာ မြန်မာ နဲ့ အင်္ဂလိပ်) သုံးတဲ့အခါ font တွေ ထိန်းချုပ်ရတာ ပိုရှုပ်ထွေးပါတယ်။
> 
နမူနာ (၂): နည်းလမ်းအသစ် (ခေတ်မီ အကြံပြုနည်း)
\documentclass{article}

% 1. Babel ကို အဓိက ထောက်ပံ့သူအဖြစ် အရင်ခေါ်သည်
\usepackage[provide=*]{babel}

% 2. Font package ကို ခေါ်သည်
\usepackage{fontspec}

% 3. ဘာသာစကားများကို ကြေညာပြီး import လုပ်သည်
\babelprovide[main, import]{burmese}
\babelprovide[import]{english} % ဒုတိယ ဘာသာစကား

% 4. Font များကို သတ်မှတ်သည်
% အဓိက font (main language ဖြစ်တဲ့ မြန်မာစာက ဒါကို သုံးမည်)
\setmainfont{Padauk} 

% အင်္ဂလိပ်စာအတွက် သီးသန့် font သတ်မှတ်ခြင်း (ဒါက နည်းသစ်ရဲ့ အားသာချက်)
\babelfont[english]{rm}{Times New Roman}

\begin{document}

\section{နိဒါန်း}
မင်္ဂလာပါ။ ဤသည်မှာ မြန်မာဘာသာ ဖြစ်သည်။ (\today)

% အင်္ဂလိပ်ဘာသာသို့ ခေတ္တပြောင်းသုံးခြင်း
\begin{otherlanguage}{english}
\section{Introduction}
Hello. This is English. (The date is \today)
% Font က Times New Roman ကို အလိုအလျောက် ပြောင်းသွားမည်
\end{otherlanguage}

\end{document}

> အားသာချက်: \babelprovide နဲ့ \babelfont တို့ ပေါင်းစပ်ပြီး မြန်မာစာ (Padauk font) နဲ့ အင်္ဂလိပ်စာ (Times New Roman font) တို့ကို စာတမ်းတစ်ခုတည်းမှာ အလွယ်တကူ ရောနှော သုံးစွဲနိုင်သွားပါတယ်။ ဒါဟာ ဘာသာစကားမျိုးစုံနဲ့ စာတမ်း (multilingual documents) တွေအတွက် အကောင်းဆုံး ဖြေရှင်းချက် ဖြစ်ပါတယ်။
> 
အနှစ်ချုပ်
 * \usepackage[burmese]{babel} က "ဒီမှာ မြန်မာလို သုံးမယ်" လို့ ရိုးရိုးလေး ပြောလိုက်တာပါ။
 * \babelprovide[main, import]{burmese} က "ငါ XeLaTeX/LuaLaTeX ကို သုံးနေတယ်။ မြန်မာဘာသာကို အဓိကဘာသာစကားအဖြစ် သတ်မှတ်မယ်။ သူ့အတွက် font တွေ၊ စည်းမျဉ်းတွေကို fontspec နဲ့ ချိတ်ဆက်ပြီး စီမံခန့်ခွဲနိုင်အောင် အကုန် import လုပ်ထားလိုက်" လို့ အသေးစိတ် ညွှန်ကြားလိုက်တာပါ။
ရှင်းလင်းပြည့်စုံမယ်လို့ မျှော်လင့်ပါတယ်ခင်ဗျာ။
\babelfont command ကို အသုံးပြုပြီး ဘာသာစကားအလိုက် font တွေကို ဘယ်လို အသေးစိတ် ထိန်းချုပ်ရမလဲဆိုတာကို နမူနာတွေနဲ့  ရှင်းပြစေချင်ပါသေးလားခင်ဗျာ။

---

ဒါက အလွန်အသုံးဝင်ပြီး စွမ်းအားမြင့်တဲ့ command တစ်ခုပါပဲ။ \babelfont ကို ဘယ်လို အသေးစိတ် သုံးရမလဲဆိုတာကို နမူနာတွေနဲ့ ရှင်းပြပေးပါမယ်။
🎯 \babelfont ဆိုတာ ဘာလဲ။
\babelfont ဆိုတာက babel package နဲ့ fontspec package တို့ကို ချိတ်ဆက်ပေးတဲ့ "ကြားခံ" command တစ်ခုပါ။
သူ့ရဲ့ အဓိက ရည်ရွယ်ချက်ကတော့ "ဘာသာစကား တစ်ခုချင်းစီအတွက် မတူညီတဲ့ font မိသားစု (font family) တွေကို သီးသန့် သတ်မှတ်ပေးဖို့" ဖြစ်ပါတယ်။
ဥပမာ-
 * မြန်မာစာ ရေးတဲ့အခါ Padauk နဲ့ Pyidaungsu font တွေကို သုံးမယ်။
 * အင်္ဂလိပ်စာ ရေးတဲ့အခါ Times New Roman နဲ့ Arial font တွေကို သုံးမယ်။
 * ဂျပန်စာ ရေးတဲ့အခါ Meiryo font ကို သုံးမယ်။
ဒါတွေအားလုံးကို စာတမ်းတစ်ခုတည်းမှာ အလိုအလျောက် အလွယ်တကူ ပြောင်းလဲနိုင်အောင် \babelfont က ကူညီပေးပါတယ်။
⚠️ မရှိမဖြစ် လိုအပ်ချက်များ (Prerequisites)
\babelfont ကို အသုံးမပြုခင်၊ သင့် document ရဲ့ ထိပ်ပိုင်း (Preamble) မှာ အောက်ပါအချက်တွေ ပြည့်စုံနေဖို့ လိုအပ်ပါတယ်-
 * Unicode Engine: XeLaTeX သို့မဟုတ် LuaLaTeX နဲ့ compile လုပ်ရပါမယ်။ (ဒါက မဖြစ်မနေပါ)
 * fontspec Package: \usepackage{fontspec} ကို ခေါ်ထားရပါမယ်။
 * babel Package: \usepackage[provide=*]{babel} ကို ခေါ်ထားရပါမယ်။
 * \babelprovide: ကိုယ်သုံးမယ့် ဘာသာစကားတွေကို \babelprovide[import]{...} နဲ့ ကြေညာထားပြီးသား ဖြစ်ရပါမယ်။
<!-- end list -->
\documentclass{article}
\usepackage[provide=*]{babel}
\usepackage{fontspec}

% ဘာသာစကားများကို ကြေညာခြင်း
\babelprovide[main, import]{burmese}
\babelprovide[import]{english}

ဒီအဆင့်တွေ ပြီးမှ \babelfont ကို စတင် အသုံးပြုနိုင်မှာ ဖြစ်ပါတယ်။
⚙️ အခြေခံ သုံးစွဲပုံ (Basic Syntax)
\babelfont ရဲ့ အဓိက ပုံစံက-
\babelfont[<ဘာသာစကား>]{<font-အမျိုးအစား>}{<font-အမည်>}

အဓိပ္ပာယ် ဖွင့်ဆိုချက်:
 * [<ဘာသာစကား>] (Language):
   * ဒါက \babelprovide မှာ သုံးခဲ့တဲ့ ဘာသာစကား အမည် (ဥပမာ burmese, english, french) ဖြစ်ပါတယ်။
   * မှတ်ချက်: ဒီ [...] ကို မထည့်ဘဲ သုံးခဲ့ရင် (\babelfont{...}{...})၊ ဒါက main language (အဓိက ဘာသာစကား) ကို သတ်မှတ်တာနဲ့ အတူတူပါပဲ။
 * {<font-အမျိုးအစား>} (Font Type):
   * ဒါက LaTeX မှာ သတ်မှတ်ထားတဲ့ font "shape" ၃ မျိုးပါ။
   * rm (Roman): ပုံမှန် Serif font (ဥပမာ Padauk, Times New Roman)။ \textrm{...} နဲ့ သုံးနိုင်ပါတယ်။ ဒါက စာတမ်းရဲ့ default font ပါ။
   * sf (Sans Serif): ခေတ်ပေါ် Sans Serif font (ဥပမာ Arial, Helvetica)။ \textsf{...} နဲ့ သုံးနိုင်ပါတယ်။
   * tt (Typewriter): Monospace font (ဥပမာ Courier New, Consolas)။ \texttt{...} နဲ့ သုံးနိုင်ပါတယ်။
 * {<font-အမည်>} (Font Name):
   * သင့်ကွန်ပျူတာမှာ install လုပ်ထားတဲ့ font ရဲ့ တိကျတဲ့ နာမည် (System Font Name) ဖြစ်ပါတယ်။ ဥပမာ "Padauk", "Pyidaungsu", "Arial"။
💡 လက်တွေ့ နမူနာများ (Practical Examples)
ကဲ... မြန်မာစာ (အဓိက) နဲ့ အင်္ဂလိပ်စာ (ဒုတိယ) ရောသုံးမယ့် document တစ်ခုကို font တွေ ဘယ်လို ထိန်းချုပ်မလဲ ကြည့်ရအောင်။
နမူနာ (၁) - ရိုးရှင်းသော နည်းလမ်း
ဒီနည်းက အသုံးအများဆုံးနဲ့ အရှင်းလင်းဆုံးပါ။
 * \setmainfont ကို သုံးပြီး အဓိက ဘာသာစကား (မြန်မာ) အတွက် default font ကို သတ်မှတ်လိုက်ပါ။
 * \babelfont ကို သုံးပြီး ဒုတိယ ဘာသာစကား (အင်္ဂလိပ်) အတွက် font ကို သီးသန့် သတ်မှတ်ပါ။
<!-- end list -->
\documentclass{article}
\usepackage[provide=*]{babel}
\usepackage{fontspec}

% ဘာသာစကား ကြေညာခြင်း
\babelprovide[main, import]{burmese}
\babelprovide[import]{english}

% --- Font သတ်မှတ်ခြင်း ---

% 1. အဓိက ဘာသာစကား (burmese) အတွက် font
% ဒါက မြန်မာစာအတွက် default 'rm' font ဖြစ်သွားမယ်
\setmainfont{Padauk} 

% 2. ဒုတိယ ဘာသာစကား (english) အတွက် font
% \babelfont[english]{rm}{...} လို့ သုံးတာနဲ့ အတူတူပါပဲ
\babelfont[english]{rm}{Times New Roman}

\begin{document}

% --- မြန်မာစာ (Padauk font နဲ့ ပြမည်) ---
\section{နိဒါန်း}
ဤသည်မှာ Padauk font ဖြင့် ရေးသားထားသော မြန်မာစာ ဖြစ်သည်။

% --- အင်္ဂလိပ်စာ (Times New Roman font သို့ အလိုအလျောက် ပြောင်းသွားမည်) ---
\begin{otherlanguage}{english}
\section{Introduction}
This text is automatically switched to Times New Roman font.
\end{otherlanguage}

% --- မြန်မာစာ (Padauk font သို့ အလိုအလျောက် ပြန်ပြောင်းသွားမည်) ---
\section{အချုပ်}
ယခု မြန်မာဘာသာသို့ ပြန်ရောက်ပါပြီ။

\end{document}

နမူနာ (၂) - အသေးစိတ် ထိန်းချုပ်သော နည်းလမ်း (rm, sf, tt အားလုံးသုံးခြင်း)
ဒီနမူနာမှာ ဘာသာစကား ၂ ခုလုံးအတွက် rm, sf, tt font တွေကို အသေးစိတ် သတ်မှတ်ပြပါမယ်။
\documentclass{article}
\usepackage[provide=*]{babel}
\usepackage{fontspec}

% ဘာသာစကား ကြေညာခြင်း
\babelprovide[main, import]{burmese}
\babelprovide[import]{english}

% --- Font သတ်မှတ်ခြင်း ---

% === မြန်မာဘာသာ (Main Language) အတွက် Font များ ===
% 'rm' (Default Font) အတွက် Pyidaungsu
\babelfont[burmese]{rm}{Pyidaungsu}
% 'sf' (Sans Serif) အတွက် Padauk
\babelfont[burmese]{sf}{Padauk}
% 'tt' (Monospace) အတွက် (သင့်တော်တာ မရှိလျှင် default ကိုပဲ ပြန်သုံးတတ်သည်)
% ဥပမာ - \babelfont[burmese]{tt}{Some_Burmese_Mono_Font} 

% === အင်္ဂလိပ်ဘာသာ (Secondary Language) အတွက် Font များ ===
% 'rm' (Default Font) အတွက် Times New Roman
\babelfont[english]{rm}{Times New Roman}
% 'sf' (Sans Serif) အတွက် Arial
\babelfont[english]{sf}{Arial}
% 'tt' (Monospace) အတွက် Courier New
\babelfont[english]{tt}{Courier New}


\begin{document}

% --- မြန်မာဘာသာ (Pyidaungsu, Padauk font များ သုံးမည်) ---
\section{မြန်မာဘာသာ Font စမ်းသပ်ချက်}

ဤသည်မှာ ပုံမှန် `rm` font (Pyidaungsu) ဖြစ်သည်။ \par
\textsf{ဤသည်မှာ `sf` (Sans Serif) font (Padauk) ဖြစ်သည်။} \par
\texttt{ဤသည်မှာ `tt` (Monospace) font ဖြစ်သည်။} \par

% --- အင်္ဂလိပ်ဘာသာ (TNR, Arial, Courier font များ သုံးမည်) ---
\begin{otherlanguage}{english}
\section{English Font Test}

This is the normal `rm` font (Times New Roman). \par
\textsf{This is the `sf` (Sans Serif) font (Arial).} \par
\texttt{This is the `tt` (Monospace) font (Courier New).}
\end{otherlanguage}

\end{document}

ဒါက ဘယ်လို အလုပ်လုပ်သလဲ။
 * သင်က \begin{otherlanguage}{english} လို့ ရိုက်လိုက်တာနဲ့ babel က "အိုကေ... အခု အင်္ဂလိပ်စာ အလှည့်" ဆိုတာ သိသွားပါတယ်။
 * ချက်ချင်းပဲ fontspec ကို "ဟေ့... အင်္ဂလိပ်စာအတွက် သတ်မှတ်ထားတဲ့ font တွေကို အဆင်သင့်လုပ်" လို့ ပြောလိုက်ပါတယ်။
 * fontspec က \babelfont[english]{rm}{Times New Roman}၊ \babelfont[english]{sf}{Arial} စတဲ့ ညွှန်ကြားချက်တွေကို ပြန်ရှာပြီး လက်ရှိ font setting တွေကို အဲဒီ font တွေနဲ့ အစားထိုး လိုက်ပါတယ်။
 * \end{otherlanguage} ကို တွေ့တဲ့အခါ၊ babel က main language (မြန်မာ) ကို ပြန်ပြောင်းပြီး fontspec ကိုလည်း \babelfont[burmese]{...} မှာ သတ်မှတ်ထားတဲ့ Pyidaungsu နဲ့ Padauk font တွေကို ပြန်ပြောင်းခိုင်းပါတယ်။
ဒီနည်းလမ်းနဲ့ ဘာသာစကား ဘယ်နှမျိုးပဲ သုံးသုံး၊ တစ်ခုချင်းစီရဲ့ font တွေကို \babelfont သုံးပြီး သပ်သပ်ရပ်ရပ် စီမံခန့်ခွဲနိုင်မှာ ဖြစ်ပါတယ်။
ရှင်းလင်းပြည့်စုံမယ်လို့ မျှော်လင့်ပါတယ်ခင်ဗျာ။
မြန်မာဘာသာ LaTeX သုံးစွဲမှုနဲ့ ပတ်သက်ပြီး \section ခေါင်းစဉ်တွေရဲ့ font ကို သီးသန့် ဘယ်လို ပြောင်းရမလဲ ဆိုတာမျိုးတွေကို ဆက်လက် သိရှိချင်ပါသေးလားခင်ဗျာ။

---

သင်ပေးလိုက်တဲ့ \babelfont{rm}{Myanmar Text} command လေးက ဘာကိုဆိုလိုသလဲဆိုတာကို အတိအကျ ရှင်းပြပေးပါမယ်။
ဒီ command က babel နဲ့ fontspec ကို ဒီလို ညွှန်ကြားလိုက်တာပါ-
> "ဒီစာတမ်းရဲ့ အဓိက ဘာသာစကား (main language) အတွက် ပုံမှန် စာလုံး (Roman/rm) အဖြစ် 'Myanmar Text' ဆိုတဲ့ font ကို အသုံးပြုပါ"
> 
အသေးစိတ် ရှင်းလင်းချက်
ဒီ command ကို နားလည်ဖို့ အပိုင်း ၃ ပိုင်း ခွဲကြည့်ရပါမယ်။
 * \babelfont
   * ဒါက babel package ကနေ fontspec ကို "ဘာသာစကားအလိုက် font သတ်မှတ်ပေးပါ" လို့ ခိုင်းစေတဲ့ command ဖြစ်ပါတယ်။
 * {rm}
   * ဒါက "Roman" (သို့မဟုတ်) ပုံမှန် စာလုံး အမျိုးအစားကို ရည်ညွှန်းပါတယ်။ စာတမ်းတစ်ခုရဲ့ အဓိက စာသားတွေအားလုံး (body text) ကို ဒီ rm font နဲ့ ရေးသားတာပါ။ (တခြားအမျိုးအစားတွေကတော့ sf (Sans Serif) နဲ့ tt (Monospace) တို့ ဖြစ်ကြပါတယ်)။
 * {Myanmar Text}
   * ဒါက သင့်ကွန်ပျူတာထဲမှာ install လုပ်ထားတဲ့ font ရဲ့ တိကျတဲ့ နာမည် ဖြစ်ပါတယ်။ ဒီနေရာမှာ "Myanmar Text" (Microsoft Windows မှာ ပါဝင်တဲ့ font) ကို သုံးဖို့ သင်က ရွေးချယ်လိုက်တာပါ။
❓ ဘာကြောင့် "Main Language" အတွက် ဖြစ်သွားတာလဲ။
သင် သတိထားမိမှာပါ၊ \babelfont ရဲ့ ရှေ့မှာ [burmese] ဒါမှမဟုတ် [english] လို ဘာသာစကားကို သတ်မှတ်တဲ့ [...] မပါပါဘူး။
\babelfont command မှာ ဒီလို [...] (optional argument) မပါခဲ့ရင်၊ babel က ဒါဟာ [main] လို့ ကြေညာထားတဲ့ အဓိက ဘာသာစကား အတွက် ညွှန်ကြားချက်ပဲလို့ အလိုအလျောက် သတ်မှတ်လိုက်ပါတယ်။
လက်တွေ့ နမူနာ (Preamble)
ဒီ command က preamble (စာတမ်းရဲ့ ထိပ်ပိုင်း) မှာ ဘယ်လို အလုပ်လုပ်သလဲဆိုတာ ကြည့်ပါ။
\documentclass{article}
\usepackage[provide=*]{babel}
\usepackage{fontspec}

% 1. မြန်မာစာကို 'main' language အဖြစ် ကြေညာ
\babelprovide[main, import]{burmese}
% 2. အင်္ဂလိပ်စာကို ဒုတိယ ဘာသာစကား အဖြစ် ကြေညာ
\babelprovide[import]{english}

% --- Font သတ်မှတ်ခြင်း ---

% 3. သင်မေးခဲ့သော Command
% [main] language (burmese) ရဲ့ 'rm' font ကို 'Myanmar Text' သတ်မှတ်
\babelfont{rm}{Myanmar Text}

% 4. အင်္ဂလိပ်စာအတွက် 'rm' font ကို 'Times New Roman' သတ်မှတ်
\babelfont[english]{rm}{Times New Roman}

% --- စာတမ်း အစ ---
\begin{document}

% ဤစာသားများသည် 'Myanmar Text' font ဖြင့် ပေါ်မည်။
\section{နိဒါန်း}
မင်္ဂလာပါ။ ဤသည်မှာ အဓိက ဘာသာစကား ဖြစ်သည်။

% ဤစာသားများသည် 'Times New Roman' font ဖြင့် ပေါ်မည်။
\begin{otherlanguage}{english}
\section{Introduction}
Hello. This text will use Times New Roman.
\end{otherlanguage}

\end{document}

💡 အရေးကြီးသော မှတ်ချက် (vs \setmainfont)
သင်သုံးလိုက်တဲ့ \babelfont{rm}{Myanmar Text} command ဟာ \setmainfont{Myanmar Text} command နဲ့ အလွန် ဆင်တူပါတယ်။
main language တစ်ခုကို ကြေညာထားပြီးတဲ့အခါ၊ အဲဒီ main language ရဲ့ rm font ကို သတ်မှတ်တာဟာ \setmainfont နဲ့ သတ်မှတ်တာနဲ့ အတူတူနီးပါးပါပဲ။
ဒါကြောင့် လူအများစုက ပိုရှင်းလင်းအောင် ဒီလို ရေးသားလေ့ရှိကြပါတယ်-
% --- ပိုမို ရှင်းလင်းသော နည်းလမ်း ---

% 1. အဓိက font (main language အတွက်) ကို \setmainfont နဲ့ သတ်မှတ်
\setmainfont{Myanmar Text}

% 2. တခြား ဘာသာစကားတွေကိုမှ \babelfont နဲ့ သီးသန့် သတ်မှတ်
\babelfont[english]{rm}{Times New Roman}

ဒီနည်းလမ်း ၂ ခုစလုံးက ရလဒ် အတူတူနီးပါး ထွက်မှာ ဖြစ်ပေမယ့်၊ ဒုတိယနည်း ( \setmainfont သုံးတဲ့နည်း) က ပိုပြီး ဖတ်ရှုရ ရှင်းလင်းလေ့ရှိပါတယ်ခင်ဗျာ။
မြန်မာစာအတွက် \textsf (Sans Serif) သုံးချင်ရင် ဘယ်လို သတ်မှတ်ရမလဲဆိုတာကို \babelfont သုံးပြီး ဆက်လက် လေ့လာချင်ပါသလားခင်ဗျာ။
