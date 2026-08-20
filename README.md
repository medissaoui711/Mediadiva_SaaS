> 🔒 **Commercial / Closed-Source Notice:**  
> هذا المستودع مخصص لتوثيق المعمارية العامة ومصمم لتوضيح الهيكلية التقنية لمنصة **Mediadiva**. الشفرة المصدرية (Source Code) والأنظمة الخلفية محفوظة في مستودعات خاصة (Private Repositories).
> 
# 🚀 Mediadiva - Next-Gen North African Freelance Engine
> **Enterprise SaaS Platform Architecture & Multi-Role Workspace Solution**

![Version](https://img.shields.io/badge/version-1.0.0-cyan)
![License](https://img.shields.io/badge/license-MIT-blue)
![Architecture](https://img.shields.io/badge/Architecture-Role--Based_SaaS-indigo)
![Coverage](https://img.shields.io/badge/Market-North_Africa_&_MENA-emerald)

ميدياتيفا هي منصة وساطة رقمية وسوق عمل حر مخصص لمنطقة شمال إفريقيا (تونس، الجزائر، المغرب، مصر، ليبيا، موريتانيا)، تعتمد على معمارية معزولة الأدوار (Role-Based SaaS) وقواعد التوثيق المكتوب وقفل العقود عبر خزانة الضمان المالي (Escrow Ledger).

---

## 📸 معاينة واجهة المنصة العامة (Public Marketplace Preview)

![Mediadiva Marketplace UI](docs/assets/marketplace-preview.jpg)

> **ملاحظة معمارية:** تعرض الواجهة المشاريع النشطة وشارات الثقة الإقليمية قبل توجيه المستخدم إلى لوحة التحكم المخصصة بحسب دوره (Client / Freelancer).



## 🛠️ التكنولوجيا المستخدمة (Tech Stack)

| الطبقة | التقنيات المستخدمة |
| :--- | :--- |
| **Frontend Framework** | React 18, Vite, TypeScript |
| **Styling & UI** | Tailwind CSS, Lucide React Icons |
| **State Management** | React Context / Zustand |
| **Backend & Database** | Node.js (Express), PostgreSQL / Supabase |
| **Security & Auditing** | Row Level Security (RLS), AI Message Filters |
| **AI Agents & Models** | Gemini LLM API, LangChain, RAG Pipelines |

---

## 📐 الهيكلية المعمارية لتجربة المستخدم (Role-Based Architecture)

تعتمد المنصة على فصل كلي بين 3 عوالم معزولة برمجياً:

```text
[Mediadiva Ecosystem]
 │
 ├── 🌐 Public Landing Page (صفحة الهبوط العامة)
 │    ├── Multi-Currency (TND / USD / EUR) & Multi-Lang (AR / FR / EN)
 │    ├── Live Featured Projects Feed
 │    ├── Regional Footprint (North Africa Badges)
 │    └── Interactive Sandbox Modal (Role Selector)
 │
 ├── 💼 Client Workspace (لوحة تحكم العميل)
 │    ├── Active Contracts & Posted Projects
 │    ├── Written Proposals Review Engine
 │    └── Escrow Financial Ledger
 │
 ├── 👨‍💻 Freelancer Workspace (لوحة تحكم المستقل)
 │    ├── Opportunities & Project Explorer
 │    ├── Written Plan Submission Tool
 │    └── Wallet & Payout Management
 │
 └── 🛡️ Admin HQ Dashboard (لوحة التحكم المركزية)
      ├── Disputes & Arbitration Center
      ├── Real-Time Escrow Liquidity Tracker
      └── Off-Platform AI Message Auditor
🛡️ آليات الأمان وحماية الحقوق (Core Security Protocols)
خزانة الضمان المالي (Escrow Protection):
تُجمد أموال المشروع تلقائياً عند توقيع العقد، ولا يتم تحريرها للحساب البنكي للمستقل إلا بعد اعتماد التسليم النهائي.
قواعد التوثيق المكتوب (Plan Lock Protocol):
يلتزم المستقل بتقديم "مخطط عمل مكتوب" (Written Plan) يحتوي على المعالم والمخرجات دقيقة الصياغة قبل قفل العقد لمنع الخلافات.
الرقابة الذكية على الرسائل (AI Moderation):
محرك فحص تلقائي يمنع مشاركة وسائل الدفع أو الاتصال الخارج عن نطاق المنصة لحماية حقوق المستحقين.
📂 دليل الهيكل البرمجي (Directory Structure)
mediadiva-platform/
├── src/
│   ├── components/
│   │   ├── landing/          # مكونات صفحة الهبوط العامة
│   │   ├── client/           # لوحة تحكم وإدارة العميل
│   │   ├── freelancer/       # سوق العمل ومحفظة المستقل
│   │   └── admin/            # مركز التحكيم والرقابة المركزية
│   ├── types/                # تعريفات TypeScript الشاملة
│   ├── services/             # ربط الـ APIs والخزانة المالية
│   └── App.tsx               # محرك التوجيه وإدارة الحالات (Routing & State)
├── public/                   # الوسائط والشارات البصرية
├── docs/                     # التوثيق المعماري والدليل الفني
└── README.md                 # دليل المنصة الموحد

⚡ التشغيل المحلي للمشروع (Local Setup)
# 1. استنساخ المستودع
git clone [https://github.com/your-username/mediadiva-platform.git](https://github.com/your-username/mediadiva-platform.git)

# 2. الدخول لمجلد المشروع
cd mediadiva-platform

# 3. تثبيت الاعتمادات
npm install

# 4. تشغيل خادم التطوير المحلي
npm run dev

📄 الترخيص (License)
​هذا المشروع مرخص تحت رخصة MIT License - راجع ملف LICENSE لمزيد من التفاصيل.


--

### الخطوات التالية لدفع الكود للمستودع:
1. قم بإنشاء ملف باسم `README.md` في المجلد الرئيسي للمشروع وضع المحتوى أعلاه فيه.
2. نفذ الأوامر التالية عبر التيرمينال لرفعه فوراً
