UPDATE AND EXPAND THE CURRENT DOCGATE MOBILE FIGMA PROTOTYPE.

DO NOT START OVER.

The current mobile visual direction is approved.

Preserve the existing DocGate visual identity, components, colors, typography, Arabic RTL behavior, navigation style, cards, mobile proportions, and the selected reference images.

This task is NOT a redesign.

This task is:

REFINE
+
CORRECT
+
COMPLETE
+
EXPAND
+
CONNECT THE FLOWS

so the Doctor/client can explore the majority of the important DocGate experience and approve both:

1. the UI/UX
2. the functional product behavior

before development continues.

==================================================
A. STRICT PROJECT BOUNDARY
==================================================

This is a FIGMA PROTOTYPE ONLY.

DO NOT:

- build backend;
- connect Supabase;
- create database logic;
- create APIs;
- modify production code;
- invent technical architecture.

Use:

Figma components
variables
variants
prototype navigation
mock state

only.

The prototype should LOOK and FEEL real,
but it does not need real backend behavior.

==================================================
B. DO NOT REGRESS THE CURRENT DESIGN
==================================================

The current DocGate mobile design is approved visually.

DO NOT randomly:

- change the color system;
- replace the typography;
- replace the navigation structure;
- redesign all cards;
- create a totally different design language;
- remove existing useful screens.

Instead:

- preserve good existing screens;
- improve weak screens;
- add missing flows;
- connect currently disconnected pages;
- add important states;
- make interactions realistic.

Use the attached reference images and existing prototype as the primary VISUAL source.

Product rules in this prompt override any incorrect behavior that might appear in a generated reference image.

==================================================
C. MAIN GOAL
==================================================

The final prototype should allow the Doctor/client to understand:

- how registration works;
- how the Doctor enters the system quickly;
- how the professional profile is completed;
- how Work Locations are managed;
- how the weekly Schedule works;
- how upcoming 30-day dates are managed;
- how exact-date exceptions work;
- how bookings are managed from Pending to Completed;
- how a booking is rescheduled;
- how patient-specific exceptions work;
- how Family Member bookings are represented;
- how payment status and Finance are separated;
- how Provider-controlled restrictions behave;
- how existing bookings are protected from schedule changes.

The Doctor should be able to approve the important workflows from the prototype.

==================================================
D. EXPERIENCE PRIORITY
==================================================

Prioritize design quality in this order:

1. Today / Doctor Home
2. Bookings
3. Schedule
4. Work Locations
5. Doctor Profile & Completion
6. Services & Prices
7. Patient controls
8. Finance

Do not make secondary settings more prominent than daily appointment management.

==================================================
E. CONSISTENT DEMO ACCOUNT
==================================================

Make the entire prototype feel like ONE coherent Doctor account.

Use consistently:

Doctor:
د. أحمد سالم

Primary specialty:
استشاري طب الباطنة والجهاز الهضمي

Country:
اليمن

Phone:
+967

Primary city:
عدن

Primary Work Location:
مركز المدينة الطبي

Location:
عدن – المنصورة

Other example Work Locations may include:

مستشفى الجمهورية التعليمي – خور مكسر

مستشفى عدن العام

مستشفى 22 مايو – المنصورة

مستشفى الصداقة التعليمي العام – الشيخ عثمان

Use realistic Yemeni context throughout.

Remove inconsistent Saudi examples such as:

جامعة الملك سعود

الهيئة السعودية للتخصصات الصحية

unless shown only as an intentionally different example.

Prefer:

جامعة عدن

and neutral/local professional data.

==================================================
F. CURRENCY
==================================================

ALL main prices and Finance values must use Yemeni Rial.

Use consistently:

ر.ي

Examples:

10,000 ر.ي

15,000 ر.ي

25,000 ر.ي

35,000 ر.ي

Do NOT show:

SAR
ر.س
ريال سعودي

in the main DocGate demo.

==================================================
G. AUTHENTICATION — RESTORE AND COMPLETE
==================================================

The WhatsApp verification page was previously removed.

RESTORE IT AND KEEP IT PERMANENTLY IN THE MAIN REGISTRATION FLOW.

Approved registration flow:

Welcome
→ Create Account
→ WhatsApp OTP Verification
→ Specialty
→ Professional Title
→ Account Ready
→ Doctor Home

Do NOT skip WhatsApp verification.

--------------------------------------------------
AUTH-01 — Welcome
--------------------------------------------------

DocGate logo.

Primary:
تسجيل الدخول

Secondary:
إنشاء حساب جديد

Optional:
استكشاف المنصة

Keep minimal.

--------------------------------------------------
AUTH-02 — Login Phone
--------------------------------------------------

Tabs:

رقم الهاتف
البريد الإلكتروني

Phone mode:

+967
رقم الهاتف
كلمة المرور

CTA:
تسجيل الدخول

Link:
نسيت كلمة المرور؟

--------------------------------------------------
AUTH-03 — Login Email
--------------------------------------------------

Email
Password

CTA:
تسجيل الدخول

--------------------------------------------------
AUTH-04 — Create Account
--------------------------------------------------

Fields:

الاسم الكامل
الدولة
رقم الهاتف
البريد الإلكتروني
كلمة المرور
تأكيد كلمة المرور

CTA:
إنشاء الحساب

Do NOT add Apple Login.

Do NOT add Google login.

Do not show social authentication unless explicitly approved later.

--------------------------------------------------
AUTH-05 — WhatsApp OTP
--------------------------------------------------

Title:

التحقق من رقم الهاتف

Text:

أرسلنا رمز التحقق المكوّن من 6 أرقام إلى رقمك عبر واتساب

Masked phone:

+967 7•• ••• •••

6 OTP cells.

Countdown:

إعادة إرسال الرمز خلال 00:60

Then:

إعادة إرسال الرمز

Also:

تغيير رقم الهاتف

Create states:

Default

Typing

Invalid:
رمز التحقق غير صحيح

Expired:
انتهت صلاحية الرمز، يرجى طلب رمز جديد

Success:
تم التحقق من رقم الهاتف

Then automatically continue.

--------------------------------------------------
AUTH-06 — Specialty
--------------------------------------------------

Title:

اختر تخصصك الطبي

Searchable selection.

This should NOT have:

تخطي الآن

Specialty is part of the essential Doctor identity.

--------------------------------------------------
AUTH-07 — Professional Title
--------------------------------------------------

Examples:

طبيب عام
أخصائي
استشاري

Do NOT make this optional in the main registration flow.

--------------------------------------------------
AUTH-08 — Account Ready
--------------------------------------------------

Short success state.

CTA:

الدخول إلى DocGate

Then Doctor Home.

==================================================
H. FORGOT PASSWORD
==================================================

Add actual clickable flows.

Phone recovery:

نسيت كلمة المرور؟
→ phone
→ WhatsApp OTP
→ new password
→ success
→ login

Email recovery:

email
→ recovery sent
→ confirmation screen

Do not expose technical authentication terms.

==================================================
I. FAST FIRST ENTRY
==================================================

The Doctor should enter the workspace BEFORE fully completing:

- license;
- certificates;
- qualifications;
- identity verification;
- work locations;
- payment.

Professional completion happens after entry.

Do not create a registration wall.

==================================================
J. DOCTOR HOME — IMPROVE OPERATIONAL VALUE
==================================================

Make Home useful for daily work.

Header:

مرحبًا د. أحمد سالم

Notifications icon.

Profile avatar.

Then:

### ملخص اليوم

مواعيد اليوم

قيد الانتظار

مؤكدة

تمت معاينتهم

Keep cards compact.

### يحتاج انتباهك

Examples:

2 حجوزات تنتظر التأكيد

ملفك المهني مكتمل بنسبة 75%

لديك 1 موعد يحتاج إجراء

### الموعد القادم

Show one prominent next appointment:

09:30 ص

محمد عبدالله

استشارة عامة

مركز المدينة الطبي

Status.

Relevant primary action.

### حجوزات اليوم

Show 2–3 compact rows.

CTA:

عرض جميع الحجوزات

### إجراءات سريعة

الحجوزات

الجدول الزمني

مواقع العمل

الملف الشخصي

Do not overload Home.

==================================================
K. NOTIFICATION CENTER
==================================================

Create Notification Center.

Examples:

حجز جديد

تم تأكيد الحجز

تمت إعادة الجدولة

تم إلغاء الحجز

تذكير بإكمال الملف

تغيير متعلق بموقع العمل

Do NOT create automatic notification settings here.

==================================================
L. PROFILE COMPLETION — MUST BE FULLY EDITABLE
==================================================

Current completion cards must not be static.

Create:

PROFILE-Completion

Progress:

75%

Cards:

المعلومات الأساسية

المعلومات المهنية

التخصص والمسمى المهني

الترخيص الطبي

المؤهلات العلمية

الشهادات

الخبرات العملية

مواقع العمل

التحقق من الهوية

EVERY card must be clickable.

Each opens an actual edit/detail screen.

After mock Save:

return to checklist

and visually update completion.

==================================================
M. BASIC INFORMATION EDIT
==================================================

Fields:

الاسم بالعربية

الاسم بالإنجليزية

رقم الهاتف

البريد الإلكتروني

نبذة مختصرة

Phone:

تم التحقق

Email may show:

غير مؤكد

with an optional:

تأكيد البريد

Email verification must not block the workspace.

==================================================
N. PROFESSIONAL INFORMATION
==================================================

Fields:

التخصص الأساسي

المسمى المهني

سنوات الخبرة

المجالات الدقيقة

اللغات

نبذة مهنية

CTA:
حفظ التغييرات

==================================================
O. QUALIFICATIONS
==================================================

Create:

Qualifications List

Example:

بكالوريوس الطب والجراحة

جامعة عدن

2018

Actions:

تعديل

حذف

CTA:

إضافة مؤهل علمي

Then Add Qualification screen.

Fields:

اسم المؤهل

الجامعة / الجهة

الدولة

سنة التخرج

التخصص

optional supporting file

Then:

Edit Qualification

and Delete confirmation.

==================================================
P. CERTIFICATES
==================================================

Create:

Certificates List

Add Certificate

Edit Certificate

Delete confirmation.

Fields:

اسم الشهادة

الجهة

السنة

الملف

==================================================
Q. MEDICAL LICENSE
==================================================

Create editable license flow.

Fields:

رقم الترخيص

الجهة المصدرة

تاريخ الإصدار

تاريخ الانتهاء if applicable

Document.

Actions:

رفع ملف

التقاط صورة

تعديل

States:

غير مكتمل

قيد المراجعة

تم التحقق

Do not block normal Dashboard use.

==================================================
R. PROFESSIONAL EXPERIENCE
==================================================

List.

Example:

مركز المدينة الطبي
طبيب باطنة
2022 – الآن

Add Experience.

Edit Experience.

Delete confirmation.

==================================================
S. PRACTICE MANAGEMENT HUB
==================================================

Create a clean screen:

إدارة الممارسة

Links:

الملف المهني

المؤهلات

الترخيص

مواقع العمل

الخدمات

الحساب والأمان

Do NOT duplicate Bookings or Schedule data.

Link to their real contextual screens.

==================================================
T. WORK LOCATIONS
==================================================

Create full flow.

Work Locations List.

Example:

مركز المدينة الطبي
عدن – المنصورة
نشط

مستشفى الجمهورية التعليمي
خور مكسر
موثق

مستشفى عدن العام
عدن
موثق

CTA:

إضافة موقع عمل

==================================================
U. ADD WORK LOCATION
==================================================

Options:

البحث عن منشأة موجودة

إضافة موقع عمل جديد

Search facility.

Select existing facility.

Manual facility.

Fields:

اسم الموقع

نوع الموقع

المحافظة

المدينة

المنطقة

العنوان

رقم التواصل

Map/location if included.

Keep easy.

==================================================
V. WORK LOCATION NAVIGATION
==================================================

Inside Work Location use:

نظرة عامة

معلومات الموقع

الجدول الزمني

الخدمات والأسعار

الحجوزات

المالية والمدفوعات

IMPORTANT order:

Schedule
→ Services & Prices
→ Bookings
→ Finance

Bookings immediately before Finance.

==================================================
W. WORK LOCATION OVERVIEW
==================================================

Use useful operational information only.

Examples:

حجوزات اليوم

مواعيد هذا الشهر

عدد الخدمات

حالة الموقع

العنوان

ساعات العمل

Do not create fake complex analytics.

==================================================
X. LOCATION INFORMATION
==================================================

Create read screen and Edit screen.

Show:

الاسم

النوع

العنوان

المدينة

المنطقة

رقم الهاتف

حالة التحقق

Map.

CTA:

تعديل معلومات الموقع

==================================================
Y. SCHEDULE — ONE CONNECTED SYSTEM
==================================================

This is CRITICAL.

Do NOT present:

Weekly Schedule

and

Monthly Schedule

as two unrelated menu items.

Inside Work Location:

الجدول الزمني

Then top segmented control:

الجدول الأسبوعي
|
الأيام الـ30 القادمة

The mental model must be:

Weekly
=
recurring base

30 Days
=
real upcoming dates derived from Weekly

Date Override
=
exception for one date

Restore Weekly
=
remove that exception

==================================================
Z. WEEKLY SCHEDULE
==================================================

Saturday through Friday:

السبت
الأحد
الاثنين
الثلاثاء
الأربعاء
الخميس
الجمعة

Each day:

يعمل

or:

إجازة أسبوعية

Use compact rows.

Example:

الخميس                     يعمل >

08:00–13:00
17:00–20:00 · فترتان

Friday:

الجمعة             إجازة أسبوعية >

Do not use giant cards.

==================================================
AA. WEEKLY DAY EDITOR
==================================================

Tap a day.

Full-screen Sheet.

Show day state.

Sessions.

Allow MULTIPLE sessions.

Example:

جلسة صباحية

08:00–13:00

15 دقيقة

جلسة مسائية

17:00–20:00

30 دقيقة

Actions:

تعديل

حذف

إضافة جلسة

==================================================
AB. SESSION EDITOR
==================================================

Fields:

اسم الجلسة — اختياري

وقت البداية

مدة الاستشارة

وقت النهاية

Capacity may be shown only as secondary concept.

IMPORTANT:

Capacity distribution remains unresolved.

Do not make Capacity control Slot ordering/display.

==================================================
AC. SLOT CALCULATION DISPLAY
==================================================

Example:

08:00 → 13:00

Duration:

15 دقيقة

Show:

عدد المواعيد الممكنة: 20

أول موعد:
08:00 ص

آخر بداية موعد:
12:45 م

13:00 is session END.

Do not show it as final appointment start.

==================================================
AD. SESSION OVERLAP VALIDATION
==================================================

Valid:

08:00–13:00

13:00–16:00

Invalid:

08:00–13:00

12:00–15:00

Inline error:

تتداخل هذه الجلسة مع جلسة أخرى.

==================================================
AE. 30-DAY SCHEDULE — FULLY EDITABLE
==================================================

This must NOT be read-only.

Doctor must be able to:

select active dates;

inspect date;

edit exact date;

close date;

mark Holiday;

add partial block;

set custom sessions;

restore Weekly;

see bookings;

see conflict protection.

==================================================
AF. 30-DAY MOBILE ENTRY
==================================================

Inside Schedule:

[الجدول الأسبوعي | الأيام الـ30 القادمة]

Selecting:

الأيام الـ30 القادمة

opens primary mobile 30-day view.

Use:

horizontal date strip

+
selected day detail.

Also provide:

عرض التقويم

for calendar overview.

==================================================
AG. 30-DAY DATE STRIP
==================================================

Example:

[س 12]
[أ 13]
[ث 14]
[ث 15]
[أ 16]
[خ 17]

Scrollable.

Selected clearly.

Show status dot/badge.

Do not overfill cells.

==================================================
AH. MONTH CALENDAR VIEW
==================================================

Create a full-screen calendar overview.

7 columns.

Arabic weekday order:

السبت
الأحد
الاثنين
الثلاثاء
الأربعاء
الخميس
الجمعة

Display month/range:

سبتمبر – أكتوبر 2026

Active dates selectable.

Outside rolling 30-day scope:

muted
non-editable.

==================================================
AI. CALENDAR STATES
==================================================

Show:

متاح

مغلق

إجازة

ممتلئ

غير معد

Also:

انتهت نافذة الحجز

as DISPLAY ONLY.

Full is system-derived.

Doctor must NOT manually select Full.

Selected is a visual layer,
not a status.

Today is also a separate visual marker.

==================================================
AJ. SELECTED DATE PANEL
==================================================

After selecting a date show:

الخميس، 17 سبتمبر

Status:

متاح

Source:

يتبع الجدول الأسبوعي

or:

لديه تعديل خاص بهذا اليوم

Then sessions.

Example:

08:00–13:00
15 دقيقة

17:00–20:00
30 دقيقة

Partial Blocks.

Booking summary.

Actions.

==================================================
AK. SELECTED DATE ACTIONS
==================================================

Primary:

تعديل هذا اليوم

Secondary menu:

إغلاق اليوم

إجازة

حظر جزء من اليوم

If overridden:

استعادة الجدول الأسبوعي

Do not display all as giant buttons.

==================================================
AL. EXACT-DATE EDIT
==================================================

Full-screen Sheet:

تعديل الخميس 17 سبتمبر

Helper:

هذا التعديل يخص هذا التاريخ فقط ولن يغيّر جدول الخميس الأسبوعي.

Options:

يعمل

مغلق

إجازة

If Working:

custom Sessions.

==================================================
AM. RESTORE WEEKLY
==================================================

If date has override:

استعادة الجدول الأسبوعي

Confirmation:

سيتم حذف التعديل الخاص بهذا التاريخ فقط وسيعود اليوم إلى جدول الخميس الأسبوعي.

Buttons:

إلغاء

استعادة الجدول

==================================================
AN. HOLIDAYS
==================================================

Create:

الإجازات والحظر

Sections:

إجازة ليوم واحد

إجازة لفترة

الحظر الجزئي

For range:

من
إلى

سبب اختياري.

Show upcoming holidays.

==================================================
AO. PARTIAL-DAY BLOCK
==================================================

Date.

From.

To.

Example:

01:00 م → 03:00 م

Reason optional.

Preview:

الفترة المحظورة

Do not automatically move booked appointments.

==================================================
AP. UNSAVED CHANGES
==================================================

Schedule must NOT autosave.

After editing show sticky bar:

لديك تغييرات غير محفوظة

Buttons:

تجاهل

حفظ التغييرات

When leaving:

لديك تغييرات غير محفوظة

هل تريد مغادرة الصفحة؟

Buttons:

البقاء

تجاهل التغييرات

==================================================
AQ. SCHEDULE CONFLICT REVIEW — MUST DEMONSTRATE
==================================================

Create working prototype flow.

Doctor changes a date with existing bookings.

Press Save.

Open:

توجد حجوزات متأثرة

Text:

يتعارض هذا التعديل مع 3 حجوزات قائمة.

Show:

09:30 ص
محمد عبدالله

10:00 ص
سارة أحمد

10:30 ص
خالد سالم

Critical message:

لن يتم إلغاء أو نقل أي حجز تلقائيًا.

Actions:

عرض الحجوزات المتأثرة

العودة لتعديل الجدول

NO:

حفظ على أي حال

for invalid conflict.

==================================================
AR. CENTER CONFIRMATION POLICY
==================================================

Use ONLY the currently approved time model.

Options:

تأكيد فوري

تأكيد في المركز

If Confirm At Center:

وقت تأكيد الحجز في المركز

Options:

في أي وقت قبل الموعد

في وقت محدد

خلال فترة زمنية

==================================================
AS. SPECIFIC CONFIRMATION TIME
==================================================

Example:

09:00 ص

Summary:

يجب على المريض تأكيد حجزه في المركز الساعة 09:00 ص.

==================================================
AT. CONFIRMATION RANGE
==================================================

From:

08:00 ص

To:

10:00 ص

Summary:

يمكن للمريض تأكيد حجزه في المركز من 08:00 ص إلى 10:00 ص.

DO NOT use:

30/60/90/120 minutes

24 hours

6 hours

DO NOT add automatic cancellation after missing the confirmation window.

==================================================
AU. SERVICES & PRICES
==================================================

Keep inside Work Location.

Examples:

استشارة عامة
15,000 ر.ي
30 دقيقة

متابعة
10,000 ر.ي
20 دقيقة

استشارة تخصصية
25,000 ر.ي
30 دقيقة

استشارة مطولة
35,000 ر.ي
45 دقيقة

Create:

Services List

Add Service

Edit Service

Delete/Deactivate confirmation.

==================================================
AV. BOOKINGS — HIGH PRIORITY
==================================================

Bookings are for CURRENT Work Location only.

Example page:

حجوزات مركز المدينة الطبي

Keep:

date strip

counters

search

filters

booking list.

==================================================
AW. BOOKING COUNTERS
==================================================

Compact.

Selected date scope.

Show:

الإجمالي

قيد الانتظار

مؤكد

مكتمل

Keep Cancelled / No-show available but not necessarily top counters.

==================================================
AX. BOOKING SEARCH
==================================================

Placeholder:

ابحث باسم المريض أو رقم الحجز

==================================================
AY. BOOKING FILTERING — MUST IMPROVE
==================================================

Add visible button:

تصفية

Show active count:

تصفية 2

Tap opens Bottom Sheet.

==================================================
AZ. FILTER SHEET
==================================================

### الحالة

قيد الانتظار

مؤكد

تم تسجيل الوصول

الزيارة جارية

مكتمل

ملغي

لم يحضر

### حالة الدفع

غير مدفوع

مدفوع

مسترد

فشل الدفع

### طريقة الدفع

الدفع عند الزيارة

الدفع الإلكتروني

### الخدمة

Choose Work Location service.

### المستفيد

المريض نفسه

أحد أفراد الأسرة

Buttons:

إعادة ضبط

تطبيق الفلاتر

==================================================
BA. ACTIVE FILTER CHIPS
==================================================

After Apply show:

[مؤكد ×]

[الدفع عند الزيارة ×]

[استشارة عامة ×]

Also:

مسح الكل

User must be able to modify/remove filters easily.

==================================================
BB. SORT
==================================================

Simple:

ترتيب حسب

الأقرب موعدًا

الأحدث إنشاءً

اسم المريض

Default:

الأقرب موعدًا

==================================================
BC. BOOKING ROW
==================================================

Prioritize:

time

patient

service

status

payment

primary action

Example:

09:30 ص               قيد الانتظار

محمد عبدالله

استشارة عامة · 30 دقيقة

الدفع عند الزيارة

[تأكيد]                      >

Do not display every action.

==================================================
BD. BOOKING DETAILS
==================================================

Use full-screen mobile Sheet.

Show:

المريض

المستفيد if family booking

رقم الحجز

التاريخ

الوقت الدقيق

الخدمة

المدة

موقع العمل

الحالة

حالة الدفع

طريقة الدفع

ملاحظة المريض

الملاحظة الداخلية

confirmation information when relevant.

Then:

PRIMARY NEXT ACTION.

Then secondary actions.

==================================================
BE. COMPLETE BOOKING LIFECYCLE — MUST SHOW
==================================================

Create clickable states.

PENDING

Primary:
تأكيد الحجز

After click:

CONFIRMED

Primary:
تسجيل الوصول

After click:

CHECKED IN

Primary:
بدء الزيارة

After click:

VISIT IN PROGRESS

Primary:
إنهاء الزيارة

After click:

COMPLETED

Read-only/history-oriented.

This is one of the MAIN CLIENT DEMO FLOWS.

==================================================
BF. DO NOT CREATE NEW PERMANENT STATUS LABELS
==================================================

Database-like canonical status vocabulary should remain conceptually:

pending

confirmed

cancelled

completed

no_show

But operational UI may display:

تم تسجيل الوصول

الزيارة جارية

as derived operational states.

Do not create a second state machine.

==================================================
BG. CHECK-IN
==================================================

Confirmation:

تسجيل وصول المريض؟

Success:

تم تسجيل الوصول

Primary changes to:

بدء الزيارة

==================================================
BH. START VISIT
==================================================

Action:

بدء الزيارة

Then:

الزيارة جارية

Primary:

إنهاء الزيارة

No clinical forms.

==================================================
BI. COMPLETE VISIT
==================================================

Confirmation:

إنهاء الزيارة؟

Then:

تمت الزيارة بنجاح

Status:

مكتمل

==================================================
BJ. NO-SHOW
==================================================

Only on eligible past appointment.

Action:

لم يحضر

Confirmation:

تسجيل المريض كـ “لم يحضر”؟

Do not show for future booking.

==================================================
BK. CANCEL BOOKING
==================================================

Create Cancel Sheet.

Show patient and appointment.

Reason.

Warning:

لن يتم حذف سجل الحجز.

If Paid:

قد يحتاج هذا الحجز إلى إجراء مالي منفصل.

Do not imply automatic refund.

==================================================
BL. MANUAL REMINDER
==================================================

Action:

إرسال تذكير

Success:

تم إرسال التذكير

Cooldown state:

تم إرسال تذكير مؤخرًا

يمكن الإرسال مرة أخرى بعد 14:32 دقيقة

Do NOT create automatic reminder scheduler/settings.

==================================================
BM. RESCHEDULE — COMPLETE FLOW
==================================================

Booking Details

→ إعادة الجدولة

→ choose date

→ choose exact available Slot

→ review

→ confirm

→ success.

Do NOT use free-form datetime input.

==================================================
BN. RESCHEDULE DATE + SLOTS
==================================================

Show selected date.

Show exact Slots:

09:00 ص

09:30 ص

10:00 ص

10:30 ص

11:00 ص

Unavailable:

disabled/non-selectable.

==================================================
BO. RESCHEDULE REVIEW
==================================================

Show:

الموعد الحالي

vs

الموعد الجديد

CTA:

تأكيد إعادة الجدولة

Then:

تمت إعادة جدولة الحجز

==================================================
BP. PROVIDER-MANAGED BOOKING VARIANT
==================================================

Create one explicit example.

Show that some actions are controlled by Provider.

For example:

تتم إدارة هذا الإجراء بواسطة المركز

or:

طلب تأكيد

طلب إلغاء

Do not make Doctor appear able to bypass Provider restrictions.

Reschedule or No-show may be disabled in this state.

Explain briefly.

==================================================
BQ. FAMILY MEMBER BOOKING
==================================================

Create one clear Booking Details example.

Account owner:

محمد عبدالله

Actual beneficiary:

سارة محمد

Relationship:

الابنة

Display:

الحجز لـ:
سارة محمد — الابنة

Do not treat the account owner as the actual care recipient.

==================================================
BR. PATIENT NOTE VS INTERNAL NOTE
==================================================

Keep separated.

ملاحظة المريض

read only.

ملاحظة داخلية

editable.

Create Edit Internal Note Sheet.

==================================================
BS. PATIENT-SPECIFIC BOOKING CONTROLS
==================================================

Do NOT show all controls in all contexts.

Show only meaningful eligible options.

==================================================
BT. AUTO-CONFIRM PATIENT
==================================================

Option:

تأكيد الحجوزات القادمة تلقائيًا

Show ONLY where useful.

If Work Location is already Instant:

hide it.

If Provider mandates center confirmation:

do not allow override.

For eligible Doctor-controlled location:

show it.

Helper:

سيتم تأكيد الحجوزات القادمة تلقائيًا عندما تسمح سياسة موقع العمل بذلك.

==================================================
BU. NO-PREPAYMENT EXCEPTION
==================================================

Keep:

السماح بالحجز بدون دفع مسبق

BUT:

hide it when Work Location already uses Pay at Visit.

hide/disable it when Provider mandates payment.

Only display where it genuinely changes behavior.

==================================================
BV. BLOCK FUTURE BOOKINGS
==================================================

Do NOT use a normal green Toggle.

This is a rare/destructive action.

Place in:

patient actions

or overflow.

Action:

منع الحجوزات المستقبلية

Open confirmation Sheet.

Text:

لن يستطيع هذا المريض إنشاء حجوزات جديدة مع هذا الطبيب.

Important:

لن تتأثر الحجوزات الحالية.

Optional:

السبب الداخلي

Danger CTA:

منع الحجوزات

Then state:

الحجوزات المستقبلية محظورة

Action:

السماح بالحجوزات مستقبلًا

==================================================
BW. FAMILY MEMBER BLOCK
==================================================

If the booking belongs to a Family Member:

wording must identify that exact beneficiary.

Example:

منع سارة محمد من الحجوزات المستقبلية

Do not imply the whole family account is blocked.

==================================================
BX. LEGACY BOOKING EDGE CASE
==================================================

Create one State-only frame:

إعادة الجدولة غير متاحة لهذا الحجز القديم.

Keep this out of main happy path.

==================================================
BY. EMERGENCY ACTIONS
==================================================

Do not create a separate emergency engine.

Emergency action leads to Schedule.

Example:

إجراء طارئ

→ فتح الجدول

→ Close day / Holiday / Partial Block

Do not automatically cancel bookings.

==================================================
BZ. FINANCE — COMPLETE AND REALISTIC
==================================================

Expand Finance significantly.

Inside current Work Location:

المالية والمدفوعات

Tabs:

نظرة عامة

المعاملات

إعدادات الدفع

Optional:

المستحقات

only where meaningful.

==================================================
CA. FINANCE OVERVIEW
==================================================

Period selector:

اليوم

هذا الأسبوع

هذا الشهر

فترة مخصصة

Default:

هذا الشهر

Cards:

إجمالي الإيرادات

الحجوزات المدفوعة

الدفع عند الزيارة

المبالغ المستردة

المبالغ المعلقة

Example:

625,000 ر.ي

==================================================
CB. PAYMENT BREAKDOWN
==================================================

حسب طريقة الدفع

الدفع عند الزيارة

الدفع الإلكتروني

For current non-eligible location:

الدفع الإلكتروني غير متاح لهذا الموقع حاليًا

==================================================
CC. ONLINE PAYMENT ELIGIBILITY
==================================================

Do not pretend every Work Location supports Online Payment.

For Doctor-added/unverified location:

الدفع عند الزيارة
متاح

الدفع الإلكتروني
غير متاح حاليًا

Helper:

يتطلب الدفع الإلكتروني أن يكون مقدم الخدمة مؤهلًا ومفعّلًا لهذه الخدمة.

Create one alternate State for eligible verified Provider.

==================================================
CD. TRANSACTIONS
==================================================

Create transaction list.

Row:

patient

service

date/time

amount

payment method

status.

Example:

محمد عبدالله

استشارة عامة

17 سبتمبر · 09:30 ص

15,000 ر.ي

الدفع عند الزيارة

مدفوع

Statuses:

مدفوع

غير مدفوع

مسترد

فشل الدفع

==================================================
CE. TRANSACTION DETAILS
==================================================

Show:

رقم الحجز

المريض

الخدمة

موقع العمل

المبلغ

طريقة الدفع

الحالة

تاريخ العملية

Reference where appropriate.

Informational only.

==================================================
CF. FINANCE FILTERS
==================================================

Bottom Sheet.

Filters:

الفترة

حالة الدفع

طريقة الدفع

الخدمة

Buttons:

إعادة ضبط

تطبيق

Keep simple.

==================================================
CG. PAYMENT SETTINGS
==================================================

Show:

الدفع عند الزيارة

الدفع الإلكتروني

Eligibility.

Do NOT show:

gateway keys

bank API setup

technical credentials.

==================================================
CH. PAID CANCELLATION FINANCE LINK
==================================================

After cancelled paid booking:

تم إلغاء الحجز

قد يحتاج هذا الحجز إلى إجراء مالي منفصل.

CTA:

عرض التفاصيل المالية

Do NOT claim automatic refund.

==================================================
CI. EMPTY STATES
==================================================

Create useful empty states for:

No bookings

No available Slots

No Work Locations

No Services

No Holidays

No Notifications

No Finance transactions.

==================================================
CJ. LOADING STATES
==================================================

Create skeleton states for:

Home

Bookings

Work Locations

Finance

==================================================
CK. ERROR STATES
==================================================

Create realistic states:

تعذر تحميل الحجوزات

تعذر تحميل البيانات المالية

رمز التحقق غير صحيح

لا توجد مواعيد متاحة

تتداخل الجلسات

فشل حفظ التعديلات

توجد حجوزات متأثرة

Use clear human Arabic.

==================================================
CL. GLOBAL BOTTOM NAVIGATION
==================================================

Keep one consistent navigation model.

Do not change bottom navigation randomly per screen.

Use maximum 5 items.

Suggested:

الرئيسية

الحجوزات

المرضى

الرسائل

المزيد

Work Location operations remain contextual inside Work Locations.

==================================================
CM. CLIENT DEMO FLOWS — CREATE START POINTS
==================================================

Create these explicit prototype flows.

----------------------------
FLOW 1 — طبيب جديد
----------------------------

Welcome

→ Create Account

→ WhatsApp OTP

→ Specialty

→ Professional Title

→ Doctor Home

→ Complete Profile later.

----------------------------
FLOW 2 — إكمال الملف
----------------------------

Home

→ Profile Completion

→ Qualifications

→ Add/Edit Qualification

→ Save

→ updated completion progress.

----------------------------
FLOW 3 — تعديل الجدول الأسبوعي
----------------------------

Work Location

→ Schedule

→ Weekly

→ Thursday

→ Add second session

→ Save.

----------------------------
FLOW 4 — تعديل يوم معين
----------------------------

Schedule

→ 30 Days

→ select Sep 17

→ Edit this Day

→ custom sessions

→ Save

→ Override shown.

----------------------------
FLOW 5 — إجازة
----------------------------

30 Days

→ date

→ Holiday

→ Save

→ calendar updates.

----------------------------
FLOW 6 — حظر جزئي
----------------------------

30 Days

→ date

→ Partial Block

→ 1 PM to 3 PM

→ Save.

----------------------------
FLOW 7 — استعادة الجدول
----------------------------

Override date

→ Restore Weekly

→ confirm

→ Weekly state restored.

----------------------------
FLOW 8 — تعارض الجدول
----------------------------

Booked day

→ Close Day

→ Save

→ Conflict Review

→ affected bookings

→ return to edit.

----------------------------
FLOW 9 — دورة الحجز اليومية
----------------------------

Bookings

→ Pending booking

→ Confirm

→ Check-in

→ Start Visit

→ Complete.

----------------------------
FLOW 10 — إعادة الجدولة
----------------------------

Booking Details

→ Reschedule

→ date

→ exact Slot

→ Review

→ Confirm

→ Success.

----------------------------
FLOW 11 — تصفية الحجوزات
----------------------------

Bookings

→ Filter

→ Pending + Pay at Visit

→ Apply

→ active chips

→ remove one chip

→ Reset.

----------------------------
FLOW 12 — Family Booking
----------------------------

Booking Details

→ show family beneficiary

→ Patient actions

→ block exact beneficiary

→ confirmation.

----------------------------
FLOW 13 — Provider Booking
----------------------------

Provider booking

→ restricted actions

→ request/managed by center state.

----------------------------
FLOW 14 — المالية
----------------------------

Work Location

→ Finance

→ Overview

→ Transactions

→ Filter

→ Transaction Detail.

==================================================
CN. CREATE CLIENT DEMO STARTING FRAMES
==================================================

Create:

START — New Doctor

START — Doctor Home

START — Work Location

START — Weekly Schedule

START — Editable 30 Days

START — Schedule Conflict

START — Today Bookings

START — Booking Lifecycle

START — Reschedule

START — Family Booking

START — Provider Booking

START — Patient Restriction

START — Finance

==================================================
CO. FEATURES THAT MUST REMAIN DEFERRED
==================================================

DO NOT implement or imply approved behavior for:

VIP

Waitlist

Queue-only booking

public Walk-in

automatic patient priority

Capacity-based Slot distribution

automatic Slot compression

Copy Week

Ramadan Schedule

appointment buffer

walk-in buffer

automatic confirmation expiry cancellation

automatic notification scheduler

payment gateway setup

large Patient CRM

==================================================
CP. CAPACITY RULE
==================================================

CAPACITY_PRODUCT_DECISION_REMAINS_DEFERRED.

Do not allow the prototype to decide how Capacity changes booking Slots.

Exact-time Slot booking remains the primary concept.

==================================================
CQ. IMPORTANT FINAL PRODUCT CHECK
==================================================

Before finishing, verify that the clickable prototype proves that the Doctor can:

✓ register with WhatsApp verification

✓ enter the workspace quickly

✓ edit profile sections

✓ add/edit qualifications

✓ add/edit certificates

✓ manage medical license

✓ manage Work Locations

✓ view and edit location details

✓ manage Services & Prices

✓ manage recurring weekly schedule

✓ use multiple sessions per day

✓ use Saturday–Friday

✓ mark Weekly Off

✓ open editable Next 30 Days

✓ select any eligible date

✓ create exact-date override

✓ close one date

✓ create one-day Holiday

✓ create Holiday range

✓ create Partial Block

✓ restore Weekly Schedule

✓ deliberately Save

✓ receive Unsaved warning

✓ see conflict protection

✓ configure center confirmation using actual clock times

✓ navigate Bookings by day

✓ search

✓ filter and edit filters

✓ see active filter chips

✓ confirm Pending booking

✓ check-in patient

✓ start visit

✓ complete visit

✓ mark No-show

✓ cancel

✓ send manual reminder

✓ reschedule using exact Slot

✓ understand Family beneficiary

✓ see Provider restrictions

✓ use eligible patient auto-confirm

✓ use eligible no-prepayment exception

✓ block future bookings safely

✓ view Finance summary

✓ filter transactions

✓ open transaction details

✓ understand payment eligibility.

==================================================
CR. FINAL UX RULE
==================================================

Do NOT make screens complicated just because the prototype is extensive.

The prototype may have MANY screens,
but each individual screen must remain SIMPLE.

Use:

progressive disclosure

Sheets

Bottom Sheets

contextual actions

one primary CTA

compact cards

clear hierarchy.

The goal is:

MORE COMPLETE EXPERIENCE

NOT

MORE CLUTTER.

==================================================
CS. FINAL VISUAL AUDIT
==================================================

All new screens must still look like the current approved DocGate prototype.

Check:

same teal palette

same typography

same radius

same card system

same icons

same AppBar

same BottomNavigation

same status badges

same Sheets

same spacing

same RTL quality.

Do not let new screens look generated independently.

==================================================
CT. FINAL OUTPUT
==================================================

Expand the current DocGate mobile prototype into approximately:

50–70 meaningful screens/states

but only where the new frame represents a real:

workflow

state

action

editor

confirmation

or error/empty condition.

Do NOT create meaningless duplicate pages to reach a number.

Create clear frame naming:

AUTH-*
HOME-*
PROFILE-*
LOCATION-*
SCHEDULE-*
SERVICE-*
BOOKING-*
PATIENT-*
FINANCE-*
STATE-*
START-*

Keep the current approved visual direction.

Do not stop until all important client-approval flows above are reachable through the prototype.

Final target:

A Doctor should be able to explore the prototype and say:

“Yes, this is how I want DocGate to work.”

without needing technical explanations.