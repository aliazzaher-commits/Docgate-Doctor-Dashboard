UPDATE AND EXPAND the CURRENT DocGate mobile Figma prototype.

DO NOT restart the design.
DO NOT redesign the approved visual style.
DO NOT remove existing useful screens or flows.

The current DocGate mobile UI direction is approved.

This task is a refinement of the existing prototype based on the following corrections.

IMPORTANT:
This is still a FIGMA FRONTEND PROTOTYPE ONLY.

NO backend.
NO Supabase.
NO APIs.
NO database.
NO production implementation.

Use realistic mock data and interactive prototype states only.

Keep the existing:
- DocGate teal identity
- Arabic RTL design
- current typography style
- card system
- mobile navigation
- spacing
- icon style
- rounded surfaces
- overall professional simplicity

The goal is to make the prototype MORE COMPLETE and MORE REALISTIC without making it harder to use.

==================================================
1. CRITICAL: RESTORE WHATSAPP CODE VERIFICATION
==================================================

The WhatsApp verification screen was accidentally removed in the latest revision.

RESTORE IT.

It is an essential part of the approved DocGate registration flow and MUST NOT be removed again.

The registration flow must be:

Welcome
→ Create Account
→ WhatsApp Code Verification
→ Specialty
→ Professional Title
→ Account Ready
→ Doctor Home

NOT:

Create Account
→ Doctor Home

and NOT:

Create Account
→ Profile Completion directly.

Create a dedicated frame:

AUTH-04-WhatsAppVerification

Arabic title:

التحقق من رقم الهاتف

Supporting copy:

أرسلنا رمز التحقق المكوّن من 6 أرقام إلى رقمك عبر واتساب

Show masked phone:

+967 7•• ••• •••

Show 6 individual OTP fields.

Example:

4  7  2  9  1  6

Include:

إعادة إرسال الرمز خلال 00:60

Then after countdown:

إعادة إرسال الرمز

Also:

تغيير رقم الهاتف

Use WhatsApp icon subtly.

Do not over-emphasize WhatsApp branding.

On successful code entry, visually demonstrate:

تم التحقق من رقم الهاتف

then transition automatically to Specialty selection.

Also create an invalid state:

رمز التحقق غير صحيح

and an expired state:

انتهت صلاحية الرمز، أرسل رمزًا جديدًا.

Keep the page extremely simple.

==================================================
2. LOGIN MUST REMAIN SIMPLE
==================================================

Keep:

رقم الهاتف
البريد الإلكتروني

as Login modes.

Phone login:

+967
رقم الهاتف
كلمة المرور

Email login:

البريد الإلكتروني
كلمة المرور

Keep:

نسيت كلمة المرور؟

Do not add OTP to normal password Login unless it is part of recovery.

WhatsApp OTP is required for:

NEW registration phone ownership verification

and phone recovery.

==================================================
3. YEMEN CONTEXT — GLOBAL MOCK DATA UPDATE
==================================================

Remove Saudi Arabia-specific mock content.

The main DocGate prototype should now use:

Country:
اليمن

Default phone code:

+967

Primary city:

عدن

Currency:

الريال اليمني

Use either:

ر.ي

or full label:

ريال يمني

Use one format consistently.

Preferred compact format:

25,000 ر.ي

Examples:

استشارة عامة
15,000 ر.ي

استشارة تخصصية
25,000 ر.ي

متابعة
10,000 ر.ي

Do NOT show:

ريال سعودي
SAR
ر.س

anywhere in the main prototype.

==================================================
4. ADEN WORK LOCATION MOCK DATA
==================================================

Replace Riyadh/Saudi hospital examples with realistic Aden examples.

Use examples such as:

مركز المدينة الطبي – عدن

مستشفى الجمهورية التعليمي – خور مكسر

مستشفى عدن العام

مستشفى 22 مايو – المنصورة

مستشفى الصداقة التعليمي العام – الشيخ عثمان

Do not invent excessive operational statistics for real hospitals.

These names are prototype context only.

The primary Doctor Work Location used throughout the main demo should be:

مركز المدينة الطبي

Location:

عدن – المنصورة

This should become the primary location used in:

Schedule
Bookings
Services & Prices
Finance

so the demonstration feels like one coherent Doctor account.

==================================================
5. WORK LOCATIONS LIST
==================================================

Update Work Locations to use Aden context.

Example cards:

مركز المدينة الطبي
عدن – المنصورة
نشط

مستشفى الجمهورية التعليمي
عدن – خور مكسر
موثق

مستشفى عدن العام
عدن
موثق

For manually-added Doctor facility examples:

show an appropriate state such as:

غير موثق بعد

Do not imply all Work Locations have identical authority/payment capabilities.

==================================================
6. PROFILE COMPLETION MUST BE INTERACTIVE
==================================================

The Profile Completion page currently looks like a static checklist.

Change it into a REAL NAVIGABLE onboarding workspace.

Title:

إكمال الملف الشخصي

Show progress:

مثلاً:
65%

Each card MUST be tappable.

Cards:

المعلومات الأساسية

المعلومات المهنية

التخصص والمسمى المهني

الترخيص الطبي

المؤهلات العلمية

الشهادات

الخبرات العملية

مواقع العمل

التحقق من الهوية والحساب

Each card opens its own editable detail screen.

Do not put all profile information in one long page.

==================================================
7. BASIC INFORMATION EDITOR
==================================================

Create:

PROFILE-EditBasicInformation

Fields:

الاسم بالعربية
الاسم بالإنجليزية
رقم الهاتف
البريد الإلكتروني
الجنس if already part of the profile
نبذة مختصرة

Phone should indicate:

تم التحقق

Email may show:

غير مؤكد

with:

تأكيد البريد

if useful.

Email verification must NOT block initial workspace usage.

Buttons:

حفظ التغييرات

==================================================
8. PROFESSIONAL INFORMATION EDITOR
==================================================

Create:

PROFILE-ProfessionalInformation

Fields:

التخصص الأساسي

المسمى المهني

سنوات الخبرة

المجالات الدقيقة

اللغات

نبذة مهنية

Allow editing.

Use small manageable forms.

==================================================
9. QUALIFICATIONS — FULL EDIT FLOW
==================================================

The card:

المؤهلات العلمية

must open a real list.

Example:

بكالوريوس الطب والجراحة

جامعة عدن

2018

Actions:

تعديل
حذف

CTA:

إضافة مؤهل علمي

Create:

PROFILE-AddQualification

Fields:

اسم المؤهل

الجامعة / الجهة التعليمية

الدولة

سنة التخرج

التخصص

optional supporting document.

Then:

حفظ المؤهل

Also create:

Edit Qualification.

==================================================
10. CERTIFICATES
==================================================

Create:

الشهادات

Cards can show:

اسم الشهادة
الجهة
السنة

Actions:

إضافة
تعديل
حذف

Do not create unnecessary certificate verification logic in the prototype.

==================================================
11. MEDICAL LICENSE
==================================================

Create a detailed Medical License screen.

Show:

رقم الترخيص

الجهة المصدرة

تاريخ الإصدار

تاريخ الانتهاء if applicable

Document.

Actions:

رفع ملف

التقاط صورة

تعديل المعلومات

Display verification state:

لم تتم المراجعة

or:

قيد المراجعة

or:

تم التحقق

according to prototype state.

The Doctor can still use his workspace while completing these steps.

==================================================
12. EXPERIENCE
==================================================

Create:

الخبرات العملية

List existing experiences.

Example:

طبيب – مركز المدينة الطبي
2022 – الآن

Action:

إضافة خبرة

Fields:

الجهة

المسمى

من

إلى / حتى الآن

وصف مختصر

Keep simple.

==================================================
13. PROFILE COMPLETION NAVIGATION
==================================================

Every Profile Completion detail screen should provide:

back navigation

Save

and clear completion state.

After saving a section:

return to Profile Completion

and visually update progress.

Example:

65%
→
72%

Use Figma prototype variables/component variants if useful.

No backend required.

==================================================
14. PROFILE COMPLETION LOGIC
==================================================

Respect the approved DocGate logic:

The Doctor can enter the workspace early.

Full professional profile completion is encouraged but does not block initial Dashboard access.

Publication/verification may require more information later.

Use helper copy such as:

يمكنك استخدام لوحة التحكم الآن، ويُفضّل إكمال ملفك المهني لزيادة موثوقية حسابك وظهوره للمرضى.

Do not use threatening/blocking copy.

==================================================
15. BOOKINGS — IMPROVE FILTERING
==================================================

The current Work Location Bookings filtering is too limited.

Improve it significantly while keeping it easy.

Screen:

حجوزات مركز المدينة الطبي

Keep the horizontal date selector.

Keep search.

Search placeholder:

ابحث باسم المريض أو رقم الحجز

Then add a clear Filter button:

تصفية

with a filter count badge.

Example:

تصفية  2

Tapping it opens a Bottom Sheet:

BOOKING-Filters

==================================================
16. BOOKINGS FILTER SHEET
==================================================

The filter system must be editable and reversible.

Use sections.

### الحالة

Multi-select:

قيد الانتظار
مؤكد
تم تسجيل الوصول
الزيارة جارية
مكتمل
ملغي
لم يحضر

Remember:

Checked-in and Visit In Progress are operational display states,
not new permanent booking-status concepts.

### حالة الدفع

الكل
غير مدفوع
مدفوع
مسترد
فشل الدفع

### طريقة الدفع

الدفع عند الزيارة
الدفع الإلكتروني

only where meaningful.

### الخدمة

Search/select services available at this Work Location.

Examples:

استشارة عامة

متابعة

استشارة تخصصية

### المستفيد

الكل

المريض نفسه

أحد أفراد الأسرة

Do not make this filter mandatory.

Bottom actions:

إعادة ضبط

تطبيق الفلاتر

Show:

عرض 8 حجوزات

if helpful.

==================================================
17. ACTIVE FILTER CHIPS
==================================================

After applying filters, show removable chips.

Example:

[مؤكد ×]

[الدفع عند الزيارة ×]

[استشارة عامة ×]

Also show:

مسح الكل

This makes filters visibly editable.

Do not hide the active filter state inside the Bottom Sheet only.

==================================================
18. DATE IS NOT A NORMAL FILTER
==================================================

Keep date navigation separate from Filter Sheet.

Use:

horizontal date strip

for operational day selection.

Example:

س 12
أ 13
ث 14
ث 15
أ 16

The selected day remains obvious.

Do not duplicate date filtering unnecessarily inside Filter Sheet.

==================================================
19. BOOKINGS COUNTERS
==================================================

Counters should react visually to the selected date.

Use compact counters:

الإجمالي

قيد الانتظار

مؤكد

مكتمل

Do not use oversized cards.

Cancelled/No-show may appear in filter/stat details when relevant.

==================================================
20. BOOKINGS SORT
==================================================

Add a simple optional sort control:

ترتيب

Options:

الأقرب موعدًا

الأحدث إنشاءً

اسم المريض

Default:

الأقرب موعدًا

Do not add complicated table sorting.

==================================================
21. SCHEDULE — CREATE LOGICAL ENTRY POINT
==================================================

Currently the 30-day Schedule should not feel like a disconnected hidden page.

Create a clear Schedule Home for each Work Location.

Example:

مركز المدينة الطبي
الجدول الزمني

At the top create segmented navigation:

الجدول الأسبوعي
الأيام الـ30 القادمة

This should be the PRIMARY logical entry.

Do not make Doctor hunt for the 30-day view.

==================================================
22. SCHEDULE HOME — WEEKLY
==================================================

Default screen:

الجدول الأسبوعي

Compact Saturday–Friday rows.

Example:

السبت                      يعمل >
08:00–13:00
17:00–20:00 · فترتان

الأحد                      يعمل >
09:00–14:00

الاثنين             إجازة أسبوعية >

Continue through Friday.

Header actions:

الأيام الـ30 القادمة

or segmented tab.

Also provide:

الإجازات والحظر

سياسة تأكيد الحجز

Do not clutter with many header buttons.

Use a secondary menu/section.

==================================================
23. MULTIPLE SESSIONS PER DAY
==================================================

Must visually support multiple Sessions.

Example:

الخميس

جلسة 1
08:00–13:00
15 دقيقة

جلسة 2
17:00–21:00
30 دقيقة

Actions:

تعديل
حذف

CTA:

إضافة جلسة

Do not overlap sessions.

Adjacent:

08:00–13:00
13:00–16:00

is allowed.

==================================================
24. SESSION EDITOR
==================================================

Use:

اسم الجلسة (اختياري)

وقت البداية

مدة الاستشارة

وقت النهاية

Do not require Capacity for Slot calculation.

Capacity behavior remains unresolved.

If Capacity is still visually displayed:

make it clearly secondary/non-authoritative.

Do not use it to hide/reorder appointment Slots.

==================================================
25. SESSION SUMMARY
==================================================

For:

08:00 → 13:00

duration:

15 minutes

show:

عدد المواعيد الممكنة: 20

أول موعد: 08:00 ص

آخر بداية موعد: 12:45 م

IMPORTANT:

The final Slot START is 12:45.

Not 13:00.

==================================================
26. 30-DAY ENTRY
==================================================

When Doctor taps:

الأيام الـ30 القادمة

open:

SCHEDULE-30Days

Primary mobile UX:

horizontal date selector

not only a tiny monthly calendar.

Example:

[س 12]
[أ 13]
[ث 14]
[ث 15]
[أ 16]
...

Auto-scroll the selected day into view.

Under it:

selected date details.

==================================================
27. OPTIONAL CALENDAR VIEW
==================================================

At the top of 30 Days add:

عرض التقويم

This opens a full-screen or large Sheet calendar.

The calendar is a SECONDARY overview.

Not the only way to select dates on mobile.

==================================================
28. 30-DAY CALENDAR STATES
==================================================

Support:

متاح

مغلق

إجازة

ممتلئ

غير معد

Display-only state when applicable:

انتهت نافذة الحجز

Selected day must be a separate visual state.

Example:

Holiday + Selected

should remain clearly Holiday,
with an extra selected border/highlight.

==================================================
29. SELECTED DAY DETAILS
==================================================

This is one of the most important Schedule screens.

Example:

الخميس، 17 سبتمبر

متاح

Then show:

يتبع الجدول الأسبوعي

or:

لديه تعديل خاص

Then sessions:

08:00–13:00
15 دقيقة
17 موعدًا متاحًا

17:00–20:00
30 دقيقة
4 مواعيد متاحة

Then optional blocks:

حظر جزئي
13:30–15:00

Then Booking summary:

5 حجوزات
3 متاحة
etc.

Be careful:

do not use unresolved Capacity semantics.

==================================================
30. SELECTED DATE ACTIONS
==================================================

Actions:

تعديل هذا اليوم

إغلاق اليوم

إضافة إجازة

حظر جزء من اليوم

If this date has an override:

استعادة الجدول الأسبوعي

Use primary/secondary menus carefully.

Do not display five giant buttons.

==================================================
31. EDIT EXACT DATE
==================================================

Create:

تعديل الخميس 17 سبتمبر

Clear helper:

هذا التعديل يخص هذا التاريخ فقط ولن يغيّر جدول الخميس الأسبوعي.

Options:

استخدام جلسات مختلفة

مغلق

إجازة

Partial block managed separately.

Allow editing sessions for that exact date.

==================================================
32. RESTORE WEEKLY
==================================================

Create confirmation:

استعادة الجدول الأسبوعي؟

Description:

سيُحذف التعديل الخاص بهذا التاريخ فقط وسيعود اليوم إلى جدول الخميس الأسبوعي.

Actions:

إلغاء

استعادة الجدول

Do not imply changes to all Thursdays.

==================================================
33. HOLIDAYS
==================================================

Create a dedicated Holidays & Blocks area.

Sections:

الإجازات القادمة

الحظر الجزئي

Add:

إجازة ليوم واحد

إجازة لفترة

For range:

من
إلى

Reason optional.

==================================================
34. PARTIAL BLOCK
==================================================

Create:

حظر جزء من اليوم

Date

من:
01:00 م

إلى:
03:00 م

Reason optional.

Preview:

المواعيد المتأثرة بهذه الفترة

Do not automatically move any booked patient.

==================================================
35. UNSAVED CHANGES
==================================================

Schedule must NOT autosave.

After an edit:

show sticky bar:

لديك تغييرات غير محفوظة

Buttons:

تجاهل

حفظ التغييرات

If navigating away:

لديك تغييرات غير محفوظة

Buttons:

البقاء

تجاهل التغييرات

==================================================
36. SCHEDULE CONFLICT REVIEW
==================================================

Keep/add this critical flow.

If Schedule modification conflicts with bookings:

open:

توجد حجوزات متأثرة

Example:

يتعارض هذا التعديل مع 3 حجوزات قائمة.

List:

09:30 ص — أحمد علي

10:00 ص — سارة محمد

10:30 ص — خالد سالم

Important:

لن يتم إلغاء أو نقل أي حجز تلقائيًا.

Actions:

عرض الحجوزات

العودة لتعديل الجدول

Do NOT provide an unsafe:

حفظ على أي حال

==================================================
37. CONFIRMATION POLICY — USE CURRENT APPROVED LOGIC
==================================================

Remove old relative controls such as:

30 minutes
60 minutes
90 minutes
120 minutes

and:

24 hours
6 hours

for center confirmation.

Use:

طريقة تأكيد الحجز

تأكيد فوري

تأكيد في المركز

When:

تأكيد في المركز

selected, show:

وقت تأكيد الحجز في المركز

Options:

في أي وقت قبل الموعد

في وقت محدد

خلال فترة زمنية

==================================================
38. CENTER CONFIRMATION TIME RANGE
==================================================

Example:

خلال فترة زمنية

من:

08:00 ص

إلى:

10:00 ص

Summary:

يمكن للمريض تأكيد حجزه في المركز من الساعة 08:00 ص إلى الساعة 10:00 ص.

No mandatory automatic cancellation toggle.

Do not show automatic cancellation as an approved feature.

==================================================
39. SERVICES & PRICES — YEMENI CURRENCY
==================================================

Update Services & Prices.

Work Location:

مركز المدينة الطبي

Example services:

استشارة عامة
15,000 ر.ي
30 دقيقة

استشارة تخصصية
25,000 ر.ي
30 دقيقة

متابعة
10,000 ر.ي
20 دقيقة

استشارة مطولة
35,000 ر.ي
45 دقيقة

Use Yemeni Rial throughout.

==================================================
40. ADD/EDIT SERVICE
==================================================

Fields:

اسم الخدمة

الوصف

مدة الموعد

السعر

الحالة

Currency display:

ر.ي

Do not add VAT/Saudi-specific terminology.

==================================================
41. FINANCE — SIGNIFICANTLY EXPAND IT
==================================================

The current Finance screen is too simplistic.

Make it realistic for a Doctor Work Location.

Title:

المالية والمدفوعات

Location selector:

مركز المدينة الطبي
عدن – المنصورة

Create tabs:

نظرة عامة

المعاملات

إعدادات الدفع

If “المستحقات” is useful in the visual prototype, it can appear only where product authority makes sense.

Do not invent a complicated payout engine.

==================================================
42. FINANCE OVERVIEW
==================================================

Show a clear period selector:

اليوم

هذا الأسبوع

هذا الشهر

فترة مخصصة

Default:

هذا الشهر

Summary cards:

إجمالي الإيرادات

الحجوزات المدفوعة

الدفع عند الزيارة

المبالغ المستردة

المبالغ المعلقة

where truthful.

Example values in Yemeni Rial:

إجمالي الإيرادات

625,000 ر.ي

الحجوزات المدفوعة

24

الدفع عند الزيارة

310,000 ر.ي

المبالغ المستردة

25,000 ر.ي

Do not show Saudi Riyal.

==================================================
43. FINANCE REVENUE BREAKDOWN
==================================================

Add a compact breakdown:

حسب طريقة الدفع

الدفع عند الزيارة

الدفع الإلكتروني

If Online Payment is not eligible for the selected Work Location:

show:

الدفع الإلكتروني غير متاح لهذا الموقع حاليًا

Do not pretend it is enabled.

==================================================
44. PAYMENT ELIGIBILITY
==================================================

Respect approved DocGate payment logic.

For Doctor-added / unverified facilities:

Online Payment should NOT appear active as if it works.

Show:

الدفع عند الزيارة
متاح

الدفع الإلكتروني
غير متاح حاليًا

Helper:

يتطلب الدفع الإلكتروني أن يكون مقدم الخدمة مؤهلًا ومفعّلًا لهذه الخدمة.

Do NOT expose technical architecture.

==================================================
45. VERIFIED PROVIDER PAYMENT STATE
==================================================

Create an alternative prototype state in:

States & Edge Cases

for a verified eligible Provider:

الدفع عند الزيارة
متاح

الدفع الإلكتروني
متاح

This demonstrates the concept without implying every location supports it.

==================================================
46. TRANSACTIONS TAB
==================================================

Create realistic transaction list.

Each row:

patient name

booking/service

date/time

amount

payment method

status

Example:

أحمد علي

استشارة عامة

17 سبتمبر · 09:30 ص

15,000 ر.ي

الدفع عند الزيارة

مدفوع

Another:

سارة محمد

استشارة تخصصية

17 سبتمبر · 10:00 ص

25,000 ر.ي

الدفع الإلكتروني

مدفوع

only in an eligible Provider demo state.

Statuses:

مدفوع

غير مدفوع

مسترد

فشل الدفع

==================================================
47. TRANSACTION DETAILS
==================================================

Tap transaction.

Open:

تفاصيل المعاملة

Show:

رقم الحجز

المريض

الخدمة

موقع العمل

المبلغ

طريقة الدفع

الحالة

تاريخ العملية

Reference if available.

This is informational.

Do not make Bookings manage settlement.

==================================================
48. FINANCIAL FILTERS
==================================================

Transactions should support simple filters:

الفترة

حالة الدفع

طريقة الدفع

الخدمة

Use Bottom Sheet similar to Booking Filters.

Buttons:

إعادة ضبط

تطبيق

Do not build accounting-grade filters.

==================================================
49. PAYMENT SETTINGS TAB
==================================================

Show only supported payment configuration.

Example for مركز المدينة الطبي:

الدفع عند الزيارة

[Enabled]

الدفع الإلكتروني

[غير متاح]

If enabled in an alternate provider state:

show it appropriately.

Do not create:

gateway credentials

credit card configuration

bank API setup

inside this prototype.

==================================================
50. FINANCE AND BOOKINGS BOUNDARY
==================================================

Booking Details may DISPLAY:

حالة الدفع

طريقة الدفع

المبلغ

but operational Finance details belong to Finance.

Do not put:

Transaction management

Refund processing

Settlement configuration

inside Booking Details.

==================================================
51. PAID BOOKING CANCELLATION UX
==================================================

If a paid booking is cancelled, show:

تم إلغاء الحجز.

ثم:

قد يحتاج هذا الحجز إلى إجراء مالي منفصل.

Button:

عرض التفاصيل المالية

This may navigate to the related transaction.

Do not claim:

تم استرداد المبلغ تلقائيًا

unless explicitly mocked as a completed refund state.

==================================================
52. FINANCE EMPTY / ERROR STATES
==================================================

Add:

لا توجد معاملات لهذه الفترة

and:

تعذر تحميل البيانات المالية

Use appropriate Retry.

==================================================
53. KEEP DAILY DOCTOR UX EASY
==================================================

Do NOT make Finance more prominent than:

Bookings

Schedule

Today.

Daily Doctor priority remains:

Today
→ Appointments
→ Schedule
→ Work Location operations
→ Finance.

==================================================
54. USE ADEN DATA CONSISTENTLY
==================================================

Throughout the prototype use coherent examples.

Doctor:

د. أحمد سالم

Primary Work Location:

مركز المدينة الطبي

عدن – المنصورة

Example patients:

محمد عبدالله

سارة أحمد

خالد سالم

نورة علي

أحمد محمد

Avoid constantly changing Doctor/location names between screens.

Make the prototype feel like ONE actual account.

==================================================
55. TIMEZONE COPY
==================================================

Use Yemen local clock times naturally.

Do not show:

Asia/Aden

everywhere.

The Doctor only needs:

09:00 ص

10:30 ص

etc.

Technical timezone should remain invisible in normal UI.

==================================================
56. PROTOTYPE FLOWS TO VERIFY
==================================================

Make sure these flows actually work:

FLOW A — NEW DOCTOR

Welcome
→ Create Account
→ WhatsApp Verification
→ Specialty
→ Professional Title
→ Doctor Home
→ Complete Profile Later

FLOW B — EDIT QUALIFICATION

Home
→ Complete Profile
→ Qualifications
→ Edit Qualification
→ Save
→ updated progress

FLOW C — SCHEDULE

Work Locations
→ مركز المدينة الطبي
→ Schedule
→ Weekly
→ 30 Days
→ select date
→ Edit this date
→ Save

FLOW D — CONFLICT

30 Days
→ select booked day
→ Close day
→ Save
→ Conflict Review
→ return to edit

FLOW E — BOOKINGS FILTER

Bookings
→ Filter
→ Pending + Pay at Visit
→ Apply
→ active chips
→ remove filter chip
→ updated list

FLOW F — FINANCE

Work Location
→ Finance
→ Overview
→ Transactions
→ Filter
→ Transaction Details
→ back

==================================================
57. DO NOT REGRESS EXISTING FEATURES
==================================================

Do not remove any of the previously approved useful screens simply because new screens are being added.

Specifically KEEP:

WhatsApp OTP

Doctor Home

Profile Completion

Doctor Profile

Work Locations

Work Location Details

Weekly Schedule

30-Day Schedule

Session Editor

Holidays / Partial Block

Confirmation Policy

Services & Prices

Bookings

Booking Details

Reschedule

Patient Restrictions

Finance

==================================================
58. STILL OUT OF SCOPE
==================================================

Do not add:

VIP

Waitlist

Queue-only booking

Walk-in system

automatic patient priority

Capacity-based Slot distribution

automatic Slot compression

Copy Week

Ramadan scheduling system

appointment buffer

payment gateway configuration

automatic notification scheduler

large Patient CRM

mandatory payment during Doctor registration

automatic cancellation after center confirmation window

==================================================
59. FINAL VISUAL PASS
==================================================

Do not make these additions look like separate modules designed by different teams.

They must still visually match the selected DocGate references.

Check:

same teal

same header

same typography

same cards

same spacing

same buttons

same status pills

same Sheets

same Bottom Navigation

same RTL behavior.

==================================================
60. FINAL PRODUCT CHECK
==================================================

Before finishing verify:

- WhatsApp OTP is back and reachable.
- Booking filters are editable and easy.
- All prices are Yemeni Rial.
- Primary facilities are in Aden.
- Profile Completion cards actually open editable screens.
- Qualifications can be add/edit/delete.
- License and certificates are editable.
- Schedule clearly lets Doctor enter Weekly and Next 30 Days.
- 30-day days are selectable and editable.
- Exact-date overrides are clear.
- Restore Weekly exists.
- Holidays and partial blocks exist.
- Conflict Review exists.
- Center confirmation uses actual clock time.
- Finance is realistic and detailed.
- Finance uses Yemeni currency.
- Payment eligibility is truthful.
- Booking management remains easier and more prominent than Finance.
- No previously approved feature was lost.

Most importantly:

The Doctor should never need technical explanation to understand the prototype.

Keep it professional, detailed, realistic, but SIMPLE TO OPERATE.