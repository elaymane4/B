---
name: "Basir Voice OS"
description: "نظام تصميم عالي التباين وسهل الوصول لمساعد أندرويد صوتي للمكفوفين يدعم الفصحى واللهجة المغربية"
---

## Overview

نظام تصميم "بصير" (Basir Voice OS) مصمم خصيصاً للمستخدمين المكفوفين وضعاف البصر مع تجربة تحكم صوتي متكاملة (Voice-First UI).
يركز الأسلوب على التباين الفائق (High-Contrast & Tactile Accessibility)، والأزرار اللمسية الضخمة (Large Touch Targets >= 64px)، والإشارات البصرية الحادة والواضحة مع ردود فعل صوتية واهتزازية (Audio-Haptic Feedback).

يدعم النظام لغتين وصوتين في آن واحد: اللغة العربية الفصحى واللهجة المغربية (الدارجة)، ويتيح للمستخدمين التحدث بحرية أو الاستماع للأوامر والأوصاف عبر قارئ الشاشة التفاعلي، مع تخصيص قسم بارز وواضح للأوامر الصوتية الجاهزة والسريعة.

## Colors

يعتمد النظام على لوحة ألوان عالية التباين تلبي معايير إمكانية الوصول العالمية (WCAG AAA) بأكثر من 7:1 للتفريق السلس لكافة عناصر الشاشة وضعاف البصر، مع خلفية داكنة مريحة وعميقة، ولمسات كهرمانية ذهبية وأزرق ساطع للتركيز والتفاعل الصوتي.

- **Primary (Electric Amber / Gold):** يعبر عن التنبيه الصوتي وحالة الاستماع النشطة وتأكيد الأوامر.
- **Secondary (Vibrant Cyan):** يُستخدم للمؤشرات الصوتية وحالة التبديل بين العربية الفصحى والدارجة المغربية.
- **Surface & Neutral:** أسود وألوان داكنة عميقة تمنع التشتت وتوفر أقصى تباين مع نصوص وأزرار ناصعة البياض والصفار.

```yaml
colors:
  accent: "#FFD026"
  success: "#10B981"
  error: "#EF4444"
  warning: "#F59E0B"
  listening: "#38BDF8"
  light:
    primary: "#0F172A"
    on-primary: "#FFFFFF"
    surface: "#FFFFFF"
    on-surface: "#090D16"
  dark:
    primary: "#FFD026"
    on-primary: "#0A0A0A"
    surface: "#0D1117"
    on-surface: "#F3F4F6"
```

## Typography

يعتمد النظام على خط **Cairo** المتميز بوضوح حروفه العربية وزواياه المفتوحة حتى على مقاسات الشاشات الصغيرة وعند التكبير الشديد (Zoom 200%)، وخط **Tajawal** للنصوص التوضيحية مع خط مونو للأرقام والرموز.

```yaml
typography:
  display-lg:
    fontFamily: "Cairo"
    fontSize: 36px
    fontWeight: 800
    lineHeight: 46px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Cairo"
    fontSize: 30px
    fontWeight: 800
    lineHeight: 40px
    letterSpacing: -0.5px
  headline-lg:
    fontFamily: "Cairo"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 38px
    letterSpacing: 0px
  headline-lg-mobile:
    fontFamily: "Cairo"
    fontSize: 24px
    fontWeight: 700
    lineHeight: 34px
    letterSpacing: 0px
  headline-md:
    fontFamily: "Cairo"
    fontSize: 20px
    fontWeight: 700
    lineHeight: 30px
    letterSpacing: 0px
  body-lg:
    fontFamily: "Tajawal"
    fontSize: 18px
    fontWeight: 600
    lineHeight: 28px
    letterSpacing: 0px
  body-md:
    fontFamily: "Tajawal"
    fontSize: 16px
    fontWeight: 500
    lineHeight: 26px
    letterSpacing: 0px
  label-lg:
    fontFamily: "Cairo"
    fontSize: 18px
    fontWeight: 700
    lineHeight: 26px
    letterSpacing: 0.2px
  label-md:
    fontFamily: "Cairo"
    fontSize: 14px
    fontWeight: 700
    lineHeight: 22px
    letterSpacing: 0.2px
```

## Layout & Spacing

يعتمد التخطيط على شبكة هاتف مرنة (Fluid Single-Column Grid) مخصصة لتطبيقات أندرويد مع مراعاة المناطق الآمنة وإمكانية لمس أي زر بسهولة تامة.
جميع العناصر التفاعلية تمتلك مساحة لمس دنيا لا تقل عن 56px، والزر الصوتي الرئيسي لا يقل عن 80px.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 32px
  page-margin: 20px
```

## Elevation & Depth

يعتمد التصميم على التباين الصريح والتأطير الحدودي المزدوج عالي الوضوح (High-Contrast Outlines & Solid Elevation) بدلاً من الظلال الباهتة أو الضبابية التي قد يصعب تمييزها على ضعاف البصر. يُعزز التراكب الحدودي بألوان براقة مع حدود 2px أو 3px عند التركيز الصوتي (Voice Focus Ring).

## Shapes

الحواف مستديرة بنعومة ملموسة تمنح إحساساً عصرياً وتساعد في تحديد حدود كل بطاقة وزر باللمس والمشاهدة.

```yaml
rounded:
  sm: 8px
  DEFAULT: 16px
  md: 20px
  lg: 24px
  xl: 32px
  full: 9999px
```

## Motion & Micro-interaction

الحركات هادفة ومرتبطة بحالة الميكروفون والاستماع الصوتي:
- تموج صوتي ناعم (Voice Wave Pulsing) ينشط عند الاستماع للأمر الصوتي.
- اهتزاز بصري خفيف ولحظي عند إتمام الأمر لتأكيد الاستجابة بجانب النطق الصوتي.

```yaml
motion:
  state-change:
    duration: 120ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 200ms
    delay: 0ms
    timingFunction: cubic-bezier(0, 0, 0.2, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.4, 0, 1, 1)
```

## Voice & Content Strategy

- **اللغة والاتجاه:** يدعم التطبيق اللغة العربية باتجاه اليمين لليسار (`dir="rtl"`).
- **نبرة الصوت (Voice Persona):** واضحة، محترمة، مفيدة وسريعة الاستجابة، تتحدث بالفصحى أو بالدارجة المغربية بطلاقة حسب رغبة المستخدم.
- **أمثلة الدارجة المغربية:**
  - "فين وصلنا؟" (تحديد الموقع الجغرافي)
  - "عيط لـ أمي" (الاتصال بالهاتف)
  - "شحال في الساعة دابا؟" (قراءة الوقت)
  - "شنو كاين فهاد الشاشة؟" (وصف محتوى الكاميرا والشاشة)
  - "قرا ليا هاد الميساج" (قراءة الرسائل الواردة)
- **أمثلة الفصحى:**
  - "اتصل بأحمد"
  - "اقرأ الرسائل غير المقروءة"
  - "افتح الكاميرا وتعرّف على المحيط"
  - "اضبط منبهاً في السابعة صباحاً"

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Chip** → `@components/chip.html`: `chip-action`, `chip-input`, `chip-with-icon`
