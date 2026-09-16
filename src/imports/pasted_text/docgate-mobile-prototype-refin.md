EXPAND AND REFINE the existing DocGate MOBILE prototype.

DO NOT restart the design from scratch.

The current prototype direction is approved.

The existing Figma Make result, the attached 5 selected UI references,
and the current DocGate visual identity must remain the visual foundation.

This is still:

MOBILE FIRST
FIGMA / FRONTEND PROTOTYPE ONLY
NO BACKEND
NO API
NO SUPABASE
NO REAL DATABASE
NO PRODUCTION LOGIC IMPLEMENTATION

Use mock/local prototype state only where interaction is needed for demonstration.

The purpose is to create the MOST COMPLETE, EASY, PROFESSIONAL and CLIENT-READY Doctor experience possible so we can show the Doctor how DocGate could work before final development.

==================================================
0. VERY IMPORTANT — DO NOT REDESIGN WHAT ALREADY WORKS
==================================================

The existing mobile screens are visually good.

Do NOT replace them with a different design language.

Instead:

- reuse them;
- refine spacing where needed;
- expand missing flows;
- add screens reachable from the current screens;
- add important states;
- make navigation complete;
- improve UX consistency.

The prototype should feel like one real mobile application.

The attached 5 images remain the primary VISUAL references.

The existing Figma Make prototype is also a reference.

Use the large 4 presentation boards as the strongest visual source because their screens are easier to read.

Use the large collage mainly to understand the broader feature coverage.

==================================================
1. PRODUCT PRIORITY
==================================================

When deciding what deserves the most attention, prioritize in this order:

1. Today / Doctor Home
2. Appointments / Bookings
3. Schedule & availability
4. Work Locations
5. Patient operational information
6. Doctor profile / professional information
7. Services & Prices
8. Payment / Finance summary
9. Secondary settings

The Doctor should be able to manage the most important daily work with as few taps as possible.

Do NOT make the product feel like a complicated hospital ERP.

==================================================
2. CORE UX PRINCIPLE
==================================================

For every screen ask:

“What does the Doctor need to know NOW?”

and:

“What is the most likely NEXT action?”

The UI should always emphasize those two things.

Avoid presenting 8 actions when only 2 are currently relevant.

Use progressive disclosure.

==================================================
3. ARABIC-FIRST MOBILE DESIGN
==================================================

Primary language:

Arabic.

RTL must be correct throughout.

Use consistent Arabic UI copy.

Prefer a modern Arabic UI font such as:

Cairo
or
IBM Plex Sans Arabic

or an equivalent clean medical UI font.

Do not generate inconsistent Arabic spelling.

Keep important product terminology exactly as described below.

==================================================
4. MOBILE FRAME
==================================================

Use approximately:

390 × 844

or equivalent modern smartphone proportions.

Use responsive Auto Layout.

Do not design based on one fixed screenshot only.

Keep safe areas and bottom navigation in mind.

==================================================
5. DESIGN SYSTEM
==================================================

Reuse / create proper reusable components.

At minimum:

AppBar
BottomNavigation
PrimaryButton
SecondaryButton
DangerButton
IconButton
TextField
PasswordField
PhoneField
OTPField
SearchField
Select
TimeInput
DateInput
Switch
RadioCard
Checkbox
StatusBadge
StatCard
InformationCard
DoctorCard
WorkLocationCard
BookingRow
BookingCard
SessionRow
ScheduleDayRow
CalendarCell
DateStripItem
Tabs
SegmentedControl
Accordion
Toast
InlineAlert
EmptyState
LoadingSkeleton
BottomSheet
FullScreenSheet
ConfirmationDialog
UnsavedChangesBar
ErrorState

Use shared variants rather than drawing new components independently on every screen.

==================================================
6. VISUAL STYLE
==================================================

Stay close to the attached references:

Primary:
DocGate dark teal / turquoise.

Secondary:
soft mint / aqua.

Background:
white / extremely light neutral or mint.

Cards:
white
subtle border
light shadow only when useful.

Rounded corners:
modern but not exaggerated.

Status colors:

Available / Success:
green

Pending:
amber

Cancelled / Error:
red

Informational:
blue

Inactive / Not configured:
neutral gray

Never rely only on color.

Always pair important statuses with a label/icon.

==================================================
7. FILE ORGANIZATION
==================================================

Organize the Figma file into:

00 — Prototype Map
01 — Foundations
02 — Components
03 — Authentication
04 — Doctor Home
05 — Practice & Profile
06 — Work Locations
07 — Schedule
08 — Services & Prices
09 — Bookings
10 — Patient Controls
11 — Finance
12 — States & Edge Cases
13 — Client Demo Flows

Do not make one enormous unorganized canvas.

==================================================
8. EXPAND THE PROTOTYPE
==================================================

The previous concept had approximately 20–21 major screens.

Expand it into a rich prototype of approximately:

45–65 meaningful frames/states

without creating unnecessary complexity.

Do NOT create pages just to increase the number.

A new frame should exist when it demonstrates:

- a real action;
- an important state;
- an important detail;
- a different workflow.

==================================================
9. AUTHENTICATION — COMPLETE FLOW
==================================================

Keep the existing visual direction.

Create / connect:

MOB-AUTH-01
Welcome

MOB-AUTH-02
Login — Phone

MOB-AUTH-03
Login — Email

MOB-AUTH-04
Forgot Password — choose/use Phone

MOB-AUTH-05
Phone Recovery WhatsApp OTP

MOB-AUTH-06
Email Recovery sent confirmation

MOB-AUTH-07
Create Account

Fields:

الاسم الكامل
الدولة
رقم الهاتف
البريد الإلكتروني
كلمة المرور
تأكيد كلمة المرور

MOB-AUTH-08
WhatsApp OTP

6 digits.

MOB-AUTH-09
Choose Medical Specialty

Searchable.

MOB-AUTH-10
Choose Professional Title

Examples:

طبيب عام
أخصائي
استشاري

MOB-AUTH-11
Account Ready / Welcome

Then enter Doctor Home immediately.

IMPORTANT:

WhatsApp OTP remains part of registration.

Email verification must NOT block initial workspace entry.

Do NOT require:

medical license
certificates
full verification
payment

before entering the Doctor workspace.

==================================================
10. DO NOT ADD MANDATORY PAYMENT ONBOARDING
==================================================

Do NOT reproduce Vezeeta's mandatory payment wall.

If a plan screen is included for presentation:

عرض الخطط

must include:

تخطي الآن

The Doctor must still be able to enter DocGate.

==================================================
11. DOCTOR HOME — MAKE THIS EXCELLENT
==================================================

The Doctor Home is one of the most important screens.

Use the existing reference as foundation but refine priorities.

Header:

مرحبًا د. أحمد

avatar

notifications.

Then create:

### TODAY OVERVIEW

مواعيد اليوم
قيد الانتظار
مؤكدة
مرضى تمت معاينتهم

Avoid meaningless vanity metrics.

### WHAT NEEDS ATTENTION

Create a compact section:

يحتاج انتباهك

Examples:

2 حجوزات تنتظر التأكيد
ملفك المهني مكتمل بنسبة 80%
لديك تعديل غير محفوظ في جدول مركز المدينة

Only show meaningful operational items.

### NEXT APPOINTMENT

Create one strong Upcoming Appointment card.

Example:

09:30 ص
محمد عبدالله
استشارة عامة
مركز المدينة الطبي

Primary action changes according to state.

### TODAY APPOINTMENTS

Show only 2–3 rows.

Then:

عرض كل الحجوزات

### QUICK ACTIONS

Prefer:

الحجوزات
الجدول
مواقع العمل
الملف الشخصي

Do NOT create too many quick actions.

==================================================
12. NOTIFICATIONS CENTER
==================================================

Add a simple Notifications screen reachable from Home.

Categories may include:

حجز جديد
تم تأكيد الحجز
تم إلغاء الحجز
تمت إعادة الجدولة
تذكير بإكمال الملف
حالة موقع العمل

Do not build a new notification configuration system.

This is only the notification inbox/display.

==================================================
13. BOTTOM NAVIGATION
==================================================

Make Bottom Navigation consistent everywhere.

Recommended:

الرئيسية
الحجوزات
المرضى
الرسائل
المزيد

BUT:

do not build a huge Patient CRM or messaging platform during this prototype.

Patients and Messages can remain simple top-level areas if already present in the current DocGate concept.

The major Work Location operations should remain contextual inside Work Locations.

==================================================
14. “MORE / PRACTICE MANAGEMENT” HUB
==================================================

This is where we should use some inspiration from the Vezeeta operational video.

Create a clean management hub:

إدارة الممارسة

Sections:

الملف الشخصي
المعلومات المهنية
المؤهلات والشهادات
الترخيص الطبي
الخبرات
مواقع العمل
الخدمات
الحساب والأمان
اللغة

Do NOT duplicate Schedule or Bookings data here.

This hub should navigate to their canonical screens.

==================================================
15. PROFESSIONAL PROFILE COMPLETION
==================================================

Expand the profile checklist.

Screen:

أكمل ملفك المهني

Progress.

Items:

المعلومات الأساسية
المعلومات المهنية
التخصص والمسمى المهني
الترخيص الطبي
المؤهلات
الشهادات
الخبرات
مواقع العمل
التحقق من الهوية

Create detail flows for important items.

==================================================
16. DOCTOR PROFILE
==================================================

Create:

Profile Overview

Edit Basic Information

Edit Professional Information

Medical License

Qualifications List

Add Qualification

Certificates List

Add Certificate

Languages

Experience

Do not put everything on one giant form.

Use small logical sections.

==================================================
17. LICENSE UPLOAD
==================================================

Create a clean license flow.

Options:

رفع ملف

التقاط صورة

Show:

اسم الوثيقة
الجهة المصدرة
رقم الترخيص
تاريخ الانتهاء if relevant

Allow:

إكمال لاحقًا

Do not block workspace navigation.

==================================================
18. WORK LOCATIONS — IMPORTANT
==================================================

Create complete Work Location management.

### LIST

Each Work Location card:

name
facility type
city/area
verification/trust status
active status

### EMPTY STATE

If Doctor has none:

لم تضف أي موقع عمل بعد

CTA:

إضافة موقع عمل

### ADD LOCATION

Provide two understandable paths:

البحث عن منشأة موجودة

إضافة موقع عمل جديد

Do not expose technical Provider identity concepts.

### SEARCH EXISTING FACILITY

Search

results

select facility

confirm relationship.

### MANUAL LOCATION

Name
Type
Country
City
Area
Address
Phone
Map / location if used

Keep the form manageable.

==================================================
19. WORK LOCATION DETAILS
==================================================

The Work Location navigation must respect:

نظرة عامة
معلومات الموقع
الجدول
الخدمات والأسعار
الحجوزات
المدفوعات

Important relative order:

Schedule
→ Services & Prices
→ Bookings
→ Payment

Bookings must be directly before Payment.

==================================================
20. WORK LOCATION OVERVIEW
==================================================

Keep it operational.

Show only helpful summaries:

حجوزات اليوم
مواعيد هذا الشهر
working status
services count
location details
verification/trust state

Do not invent excessive analytics.

==================================================
21. LOCATION INFORMATION
==================================================

Create a dedicated page:

معلومات الموقع

Show:

name
type
address
city
area
phone
map
trust/verification state

CTA:

تعديل معلومات الموقع

Then create the Edit Location screen.

==================================================
22. SCHEDULE — THIS IS A TOP PRIORITY
==================================================

The Schedule section must be the most detailed part of this prototype after Bookings.

Do not oversimplify it.

The Doctor must clearly understand:

- what his normal week looks like;
- what is happening on a specific date;
- how to change one day;
- how to add sessions;
- how to take leave;
- how changes affect existing bookings.

==================================================
23. WEEKLY RECURRING SCHEDULE
==================================================

Base recurring week:

Saturday
through
Friday.

Arabic order:

السبت
الأحد
الاثنين
الثلاثاء
الأربعاء
الخميس
الجمعة

Every day:

Working
or
Weekly Off.

A working day may contain MULTIPLE sessions.

Example:

السبت                     يعمل >
08:00–13:00
17:00–20:00
فترتان

Friday:

الجمعة              إجازة أسبوعية >

Keep mobile rows compact.

Do NOT use giant day cards.

==================================================
24. WEEKLY DAY EDITOR
==================================================

Tap a weekday.

Open full-screen editor.

Show:

Day state:

يعمل
إجازة أسبوعية

Sessions.

Example:

الجلسة الأولى
08:00–13:00
15 دقيقة

الجلسة الثانية
17:00–20:00
30 دقيقة

Actions:

تعديل
حذف
إضافة جلسة

Adjacent sessions are allowed:

08:00–13:00
13:00–16:00

Overlapping sessions are not allowed.

Show an overlap validation state.

==================================================
25. SESSION EDITOR
==================================================

Fields:

اسم الجلسة (اختياري)

وقت البداية

مدة الاستشارة

وقت النهاية

Require End in the main active prototype.

Capacity is still an unresolved product behavior.

DO NOT use Patient Capacity to calculate booking distribution.

If you visually preserve:

سعة الجلسة

treat it as optional / non-authoritative.

Do not calculate slots from Capacity.

The Slot timeline is based on:

Start
+
End
+
Consultation Duration.

Example:

08:00–13:00
15 minutes

Generate:

08:00
08:15
...
12:45

IMPORTANT:

12:45 is the last appointment START.

Not 13:00.

Show computed summary:

عدد المواعيد الممكنة
أول موعد
آخر بداية موعد

==================================================
26. CAPACITY PRODUCT NOTE
==================================================

Capacity slot-distribution behavior is NOT approved yet.

Do not make the client prototype imply:

first N slots

or:

show all then cap

or:

automatic compaction.

If needed, place this only in an internal design annotation:

CAPACITY DISTRIBUTION — PRODUCT DECISION PENDING

Do not make it part of the main Doctor demo flow.

==================================================
27. NO AUTOSAVE
==================================================

Schedule changes must feel deliberate.

After changing Schedule:

show a sticky Save Bar:

لديك تغييرات غير محفوظة

[تجاهل]
[حفظ التغييرات]

Do not simulate autosave.

==================================================
28. UNSAVED NAVIGATION WARNING
==================================================

If Doctor tries to leave:

لديك تغييرات غير محفوظة

هل تريد مغادرة الصفحة؟

Buttons:

البقاء
تجاهل التغييرات

Do not make accidental changes easy.

==================================================
29. NEXT 30 DAYS
==================================================

Create a mobile-friendly 30-day interface.

PRIMARY mobile interaction:

horizontal date strip.

Example:

[س 8]
[أ 9]
[ث 10]
[ث 11]
[...]

Auto-scroll selected date into view.

Below it:

selected date detail.

Also provide a secondary:

عرض التقويم

to open a compact monthly/calendar-style overview.

Do not force tiny calendar interactions as the only mobile method.

==================================================
30. 30-DAY CALENDAR
==================================================

Calendar states:

متاح
مغلق
إجازة
ممتلئ
غير معد

Also support display-only:

انتهت نافذة الحجز

when applicable.

Selected state must remain a separate visual layer.

Do not redefine the original status when selected.

Dates outside the active 30-day range, if shown for calendar continuity:

muted
non-interactive.

==================================================
31. SELECTED DATE DETAIL
==================================================

This is very important.

When Doctor selects a date show:

الخميس، 10 سبتمبر

State badge.

Then:

يتبع الجدول الأسبوعي

or:

لديه تعديل خاص بهذا اليوم

Sessions:

09:00–13:00
17:00–20:00

Blocks.

Bookings summary.

Available actions:

تعديل هذا اليوم
إغلاق اليوم
إجازة
حظر جزء من اليوم

If overridden:

استعادة الجدول الأسبوعي

==================================================
32. EXACT-DATE OVERRIDE
==================================================

Doctor can change one date WITHOUT altering weekly recurrence.

Create screen:

تعديل الخميس 10 سبتمبر فقط

Options:

Custom sessions

Closed

Holiday

Partial block

The UI must clearly say:

هذا التغيير يخص هذا التاريخ فقط ولن يغير جدول الخميس الأسبوعي.

==================================================
33. RESTORE WEEKLY SCHEDULE
==================================================

Create confirmation:

استعادة الجدول الأسبوعي

This will remove the special override for this date only.

It must NOT change other dates.

==================================================
34. HOLIDAYS
==================================================

Holiday manager.

Allow:

إجازة ليوم واحد

إجازة لفترة

Optional reason.

Show current/upcoming holidays.

Allow restoring/editing one date cleanly.

==================================================
35. PARTIAL-DAY BLOCK
==================================================

Create:

حظر جزء من اليوم

Date

From

To

Reason optional.

Example:

13:00 → 15:00

Show how overlapping appointment Slots visually disappear in schedule preview.

Do NOT move bookings automatically.

==================================================
36. SCHEDULE CONFLICT REVIEW — MUST ADD
==================================================

THIS IS AN IMPORTANT MISSING SCREEN.

When Doctor attempts to save a Schedule change that conflicts with existing bookings:

Do NOT silently save.

Open full-screen Conflict Review.

Title:

توجد حجوزات متأثرة

Example:

هذا التغيير يتعارض مع 3 حجوزات موجودة.

Show compact affected bookings:

09:30 — أحمد محمد
10:00 — سارة علي
10:30 — خالد عبدالله

Important message:

لن يتم إلغاء أو نقل أي حجز تلقائيًا.

Do NOT provide:

Save Anyway

if the current change is invalid.

Provide:

عرض الحجوزات المتأثرة

العودة لتعديل الجدول

This prototype must demonstrate that DocGate protects existing appointments.

==================================================
37. BOOKING CONFIRMATION POLICY
==================================================

Remove the OLD relative minute/hour concept from the current mockups.

Do NOT show:

قبل الموعد بـ30 دقيقة
60
90
120

Do NOT use:

24 hours / 6 hours

as the primary confirmation configuration.

Approved model:

طريقة تأكيد الحجز

Option A:

تأكيد فوري

Option B:

تأكيد في المركز

When Confirm At Center selected:

وقت تأكيد الحجز في المركز

Options:

في أي وقت قبل الموعد

في وقت محدد

خلال فترة زمنية

==================================================
38. CONFIRMATION — SPECIFIC TIME
==================================================

Example:

في وقت محدد

وقت التأكيد:

09:00 ص

Summary:

يجب على المريض تأكيد حجزه في المركز الساعة 09:00 ص.

==================================================
39. CONFIRMATION — TIME RANGE
==================================================

Example:

خلال فترة زمنية

من:
08:00 ص

إلى:
10:00 ص

Summary:

يمكن للمريض تأكيد حجزه في المركز من 08:00 ص إلى 10:00 ص.

Do NOT add mandatory automatic cancellation after the window.

Automatic cancellation remains a separate product decision.

==================================================
40. SERVICES & PRICES — CURRENTLY MISSING
==================================================

Add this Work Location tab.

List services.

Each row:

service name
duration
price
active/inactive

CTA:

إضافة خدمة

Create:

Add Service

Edit Service

Fields may include:

اسم الخدمة
الوصف المختصر
مدة الموعد
السعر
الحالة

Keep simple.

Do not create complex billing logic.

==================================================
41. WORK LOCATION BOOKINGS — TOP PRIORITY
==================================================

Bookings must feel like the Doctor's daily operational workspace.

Scope:

THIS Work Location only.

Do not mix bookings from unrelated locations.

==================================================
42. BOOKINGS LIST
==================================================

Use horizontal date selector.

Then compact counters:

الإجمالي
قيد الانتظار
مؤكد
ملغي

Use actual status names consistently.

Search:

ابحث باسم المريض أو رقم الحجز

Filter:

الحالة

Do not create excessive filters.

==================================================
43. BOOKING ROW
==================================================

Prioritize:

exact appointment time

patient/beneficiary name

service

status

payment state

one relevant primary action

overflow menu.

Example:

09:30 ص                    قيد الانتظار

محمد أحمد
استشارة عامة · 30 دقيقة

الدفع عند الزيارة

[تأكيد]                       >

Do not show 6 action buttons in the row.

==================================================
44. DIFFERENT BOOKING STATES
==================================================

Create realistic prototype variants.

### PENDING

Primary:

تأكيد الحجز

Secondary:

إعادة الجدولة
إلغاء
إرسال تذكير

### CONFIRMED

Primary:

تسجيل الوصول

### CHECKED IN

Primary:

بدء الزيارة

### VISIT IN PROGRESS

Primary:

إنهاء الزيارة

### COMPLETED

Read/history oriented.

### CANCELLED

Read/history oriented.

### NO-SHOW

Read/history oriented.

Do not create database-like statuses such as:

arrived
in_progress

in the Doctor-facing status vocabulary unnecessarily.

They are operational presentation states.

==================================================
45. BOOKING DETAILS
==================================================

Use Full-screen Sheet.

Display:

patient name

beneficiary name if different

booking reference

exact appointment date/time

duration

service

Work Location

booking status

payment state

patient note

internal operational note

confirmation information if relevant

Then:

Primary next action.

Then:

Secondary actions.

==================================================
46. CHECK-IN FLOW
==================================================

Create confirmation state:

تسجيل وصول المريض؟

Then success:

تم تسجيل الوصول

Booking Details changes Primary Action to:

بدء الزيارة

Keep interaction quick.

==================================================
47. START VISIT
==================================================

Tap:

بدء الزيارة

Show subtle confirmation if necessary.

Then operational state:

الزيارة جارية

Primary:

إنهاء الزيارة

Do not create unnecessary clinical forms.

==================================================
48. COMPLETE VISIT
==================================================

Confirmation:

إنهاء الزيارة؟

Then:

تمت الزيارة

Status:

مكتمل

Do not add clinical documentation unless it already belongs to another product feature.

==================================================
49. NO-SHOW
==================================================

For eligible past appointment:

لم يحضر المريض

Confirmation dialog.

Do not show No-show for a future booking.

==================================================
50. CANCELLATION
==================================================

Create Cancel Booking Sheet.

Show:

المريض
الموعد
سبب الإلغاء — optional/required depending UI pattern

Warning:

لن يتم حذف سجل الحجز.

Do not pretend a refund is automatically processed.

If Paid:

show:

قد يتطلب هذا الحجز إجراءً ماليًا منفصلًا.

Finance handles financial settlement/refund.

==================================================
51. MANUAL REMINDER
==================================================

Action:

إرسال تذكير

Success Toast:

تم إرسال التذكير.

Also create cooldown state:

تم إرسال تذكير مؤخرًا.

يمكن الإرسال مرة أخرى بعد 14:32 دقيقة.

Do not create automatic reminder settings.

Automatic location notification settings remain deferred.

==================================================
52. RESCHEDULE — IMPORTANT
==================================================

Rescheduling must use exact available Slots.

Flow:

Booking Details
→ إعادة الجدولة
→ choose date
→ choose exact Slot
→ review
→ confirm.

Show current appointment clearly.

Do NOT use free-form date/time input.

==================================================
53. RESCHEDULE DATE SCREEN
==================================================

Show compact calendar/date strip.

Select date.

Then available exact slots.

Example:

09:00
09:30
10:00
10:30
11:00

Unavailable slots should not behave like available ones.

==================================================
54. RESCHEDULE REVIEW
==================================================

Show:

الموعد الحالي

and:

الموعد الجديد

Primary:

تأكيد إعادة الجدولة

Never imply the system moved the patient automatically.

==================================================
55. RESCHEDULE SUCCESS
==================================================

Toast/success:

تمت إعادة جدولة الحجز

Show new exact appointment time.

==================================================
56. PROVIDER-MANAGED BOOKING VARIANT
==================================================

Create at least one Provider-managed Booking Details state.

Doctor should NOT visually appear able to bypass Provider authority.

Instead of direct action, where applicable use:

طلب تأكيد

طلب إلغاء

or:

تتم إدارة هذا الإجراء بواسطة المركز

Do not expose direct forbidden actions.

No-show / Reschedule can be disabled if authority is not available.

Show a concise explanation.

==================================================
57. LEGACY BOOKING EDGE STATE
==================================================

Create a small edge-case state only in States & Edge Cases:

إعادة الجدولة غير متاحة لهذا الحجز القديم.

Use:

عرض التفاصيل

and other safe actions.

Do NOT make Legacy complexity part of the normal happy path.

==================================================
58. FAMILY MEMBER BOOKINGS
==================================================

Must support actual beneficiary.

Example:

صاحب الحساب:
محمد عبدالله

الحجز لـ:
سارة محمد — الابنة

Booking list may display:

سارة محمد

with subtle:

مستفيد من حساب محمد عبدالله

Do not confuse the account owner with the patient receiving care.

==================================================
59. BOOKING NOTE
==================================================

Separate:

ملاحظة المريض

read-only

from:

ملاحظة داخلية

editable by authorized Doctor/team.

Create Edit Internal Note Sheet.

Do not create a large Patient CRM note system.

==================================================
60. PATIENT CONTROLS
==================================================

Do not call everything general “Patient Settings” without context.

Use:

إعدادات الحجز لهذا المريض

Then show only meaningful eligible options.

==================================================
61. PATIENT AUTO-CONFIRM
==================================================

Keep:

تأكيد الحجوزات القادمة تلقائيًا

BUT:

Only show when meaningful.

If Work Location is already:

Instant Confirmation

hide it because it is redundant.

If Provider has mandatory confirmation:

do not let Doctor bypass it.

For eligible Doctor-controlled Confirm At Center location:

show toggle.

Helper:

سيتم تأكيد حجوزات هذا المريض تلقائيًا عندما تسمح سياسة الموقع بذلك.

==================================================
62. NO-PREPAYMENT PATIENT EXCEPTION
==================================================

Keep capability:

السماح بالحجز بدون دفع مسبق

BUT:

Do not show it on a Pay-at-Visit location where it changes nothing.

Do not show it if Provider mandates payment.

Only show it in an eligible context.

Helper:

يُطبق هذا الاستثناء فقط عندما تسمح سياسة موقع العمل بذلك.

==================================================
63. BLOCK FUTURE BOOKINGS
==================================================

Rare/destructive action:

منع الحجوزات المستقبلية

Do not make it a prominent green toggle.

Prefer overflow action or destructive section.

Confirmation Sheet:

منع الحجوزات المستقبلية؟

Patient:

سارة محمد

Explanation:

لن يستطيع هذا المريض إنشاء حجوزات جديدة مع هذا الطبيب.

Existing bookings:

لن تتأثر الحجوزات الحالية.

Optional private reason.

Button:

منع الحجوزات

Then blocked state:

الحجوزات المستقبلية محظورة

Action:

السماح بالحجوزات مستقبلًا

==================================================
64. FAMILY MEMBER BLOCKING
==================================================

If booking is for a family member:

block that beneficiary only.

Example:

منع سارة محمد من الحجوزات المستقبلية

Do NOT show wording that suggests the entire account/family is blocked.

==================================================
65. EMERGENCY ACTION
==================================================

Can exist as a secondary option in Bookings/Schedule.

Example:

إجراء طارئ

Tap:

فتح الجدول

Then Doctor may:

إغلاق اليوم
إجازة
حظر فترة

Do NOT automatically cancel existing bookings.

==================================================
66. FINANCE
==================================================

Keep Finance visually similar to selected references.

Work Location Finance.

Possible tabs:

نظرة عامة
المعاملات
إعدادات الدفع

Show:

الإيرادات
الرصيد
المعاملات
المستحقات

Do not mix operational Booking actions into Finance.

==================================================
67. PAYMENT SETTINGS
==================================================

Display only truthful available concepts.

Possible:

الدفع عند الزيارة

الدفع الإلكتروني

Online Payment may appear unavailable.

If unavailable show:

غير متاح لهذا الموقع حاليًا

with explanation.

Do not create payment gateway setup.

==================================================
68. TRANSACTIONS
==================================================

Simple list.

Patient
date
amount
status.

Transaction Detail may show read-only operational information.

Do not invent complicated accounting tools.

==================================================
69. EMPTY STATES
==================================================

Create polished empty states for at least:

No Bookings today

No Work Locations

No Services

No available Slots

No Notifications

No Holidays

Each with appropriate CTA only where useful.

==================================================
70. LOADING STATES
==================================================

Use Skeletons for:

Home

Bookings

Work Locations

Do not show infinite spinners everywhere.

==================================================
71. ERROR STATES
==================================================

Create at least:

Data failed to load

Action failed

Schedule conflict

Invalid session overlap

OTP incorrect

No Slots available.

Use human language.

Not technical errors.

==================================================
72. FORM VALIDATION
==================================================

Show realistic examples.

Examples:

OTP incorrect

Email invalid

Passwords do not match

Session end before start

Sessions overlap

Holiday range invalid

Confirmation time range invalid

Do not use scary red walls of text.

==================================================
73. TIME PICKERS
==================================================

Time selection is important.

Use simple mobile time picker.

Consistently display example format:

09:00 ص
09:30 ص
01:00 م

Time is local to the Work Location.

Do not repeatedly expose timezone technical details.

==================================================
74. DATE PICKERS
==================================================

Use date selector appropriate for the task.

Bookings:
horizontal dates.

Schedule:
horizontal 30-day strip + optional calendar.

Reschedule:
date selection + Slots.

Holiday range:
date range picker.

Do not force one calendar component everywhere.

==================================================
75. DOCTOR DAILY DEMO FLOW
==================================================

Create a Prototype Flow named:

FLOW — يوم الطبيب

Start:

Home

→ Today Bookings

→ Booking Pending

→ Confirm

→ Check-in

→ Start Visit

→ Complete Visit

→ back to Today Bookings.

This should be one of the main flows we demonstrate to the Doctor.

==================================================
76. SCHEDULE DEMO FLOW
==================================================

Create:

FLOW — تعديل الجدول

Work Location

→ Schedule

→ Weekly Schedule

→ Edit Thursday

→ Add second session

→ Save

→ Next 30 Days

→ select date

→ create one-day override

→ Save.

==================================================
77. SCHEDULE CONFLICT DEMO
==================================================

Create:

FLOW — حماية الحجوزات

Schedule

→ edit a date with existing bookings

→ Save

→ Conflict Review

→ show affected bookings

→ return to edit.

This is important to demonstrate trust/safety.

==================================================
78. HOLIDAY DEMO FLOW
==================================================

Schedule

→ Holidays

→ Add range

→ select dates

→ optional reason

→ Save

→ show holiday on 30-day calendar.

==================================================
79. CENTER CONFIRMATION DEMO
==================================================

Work Location

→ Schedule / Confirmation Policy

→ Confirm At Center

→ During time range

→ From 08:00

→ To 10:00

→ Save

→ show human-readable summary.

==================================================
80. RESCHEDULE DEMO FLOW
==================================================

Bookings

→ Booking Details

→ Reschedule

→ date

→ exact Slot

→ review

→ confirm

→ success.

==================================================
81. PATIENT RESTRICTION DEMO
==================================================

Booking Details

→ Patient actions

→ Prevent future bookings

→ reason optional

→ confirm

→ blocked state.

For family booking use beneficiary-specific wording.

==================================================
82. PROFILE COMPLETION DEMO
==================================================

Home

→ Profile Completion

→ Professional Information

→ License

→ Qualifications

→ Work Location

→ progress updated.

Use mock progress state.

No backend required.

==================================================
83. PROTOTYPE INTERACTION ONLY
==================================================

Because this is a pure Figma prototype:

simulate state changes visually.

Examples:

Pending booking
→ Confirm
→ confirmed variant.

Do NOT create real backend.

Do NOT request database integration.

Use variables/component variants/local mock state only if helpful.

==================================================
84. CLIENT PRESENTATION MODE
==================================================

Make the prototype easy to demonstrate live.

Create clearly named starting points:

START — New Doctor

START — Doctor Home

START — Daily Appointments

START — Schedule Management

START — Work Location

START — Patient Restriction

START — Finance

The client should not need to hunt for the right screen.

==================================================
85. DO NOT OVERLOAD THE DOCTOR
==================================================

More screens do NOT mean more elements per screen.

Keep screens focused.

One screen can contain:

one primary goal
one primary CTA
a few secondary actions.

Use Sheets to reveal complexity progressively.

==================================================
86. IMPORTANT FEATURES THAT MUST NOT BE LOST
==================================================

Verify the prototype includes these agreed concepts:

AUTH
✓ Phone login
✓ Email login
✓ WhatsApp OTP
✓ Forgot password
✓ Specialty
✓ Professional title
✓ fast workspace entry
✓ professional completion later
✓ no forced payment

WORK LOCATIONS
✓ multiple locations
✓ trust/verification state
✓ overview
✓ location information
✓ Schedule
✓ Services & Prices
✓ Bookings
✓ Payment

SCHEDULE
✓ Saturday–Friday
✓ Working / Weekly Off
✓ multiple sessions/day
✓ exact start/end/duration
✓ 30-day view
✓ exact date override
✓ Closed
✓ Holiday
✓ Full
✓ Not Configured
✓ Booking Window Ended display state
✓ Restore Weekly
✓ one-day holiday
✓ holiday range
✓ partial block
✓ no autosave
✓ unsaved changes warning
✓ conflict protection
✓ actual-clock center confirmation
✓ no silent booking movement

BOOKINGS
✓ Work Location scoped
✓ search
✓ filter
✓ counters
✓ exact time
✓ pending
✓ confirmed
✓ checked-in
✓ in-visit operational state
✓ completed
✓ cancelled
✓ no-show
✓ notes
✓ reminder
✓ reschedule using exact Slot
✓ Provider authority variant
✓ family beneficiary
✓ payment display
✓ patient-specific exceptions
✓ block future bookings

FINANCE
✓ summary
✓ transactions
✓ payment eligibility/setup display
✓ separate from operational Booking management

==================================================
87. FEATURES THAT MUST REMAIN OUT OF SCOPE
==================================================

DO NOT introduce:

VIP

Waitlist

queue-only booking

Walk-in system

automatic patient priority

automatic Slot compaction

Capacity Slot distribution

Copy Week

Ramadan system

appointment buffer

walk-in buffer

payment gateway integration

automatic notification scheduler

large Patient CRM

automatic cancellation after center confirmation window

==================================================
88. IMPORTANT CAPACITY RULE
==================================================

CAPACITY_PRODUCT_DECISION_REMAINS_DEFERRED

Do not let the prototype silently decide what Capacity means.

The exact-time Schedule remains the visual booking model.

==================================================
89. NOTIFICATION RULE
==================================================

Manual Reminder can be demonstrated.

Automatic location-specific notification settings are NOT finalized.

Do not create fake notification settings.

==================================================
90. PROVIDER RULE
==================================================

Whenever the Work Location is Provider-controlled:

Doctor-specific exceptions must never visually look like they bypass mandatory Provider rules.

Use:

disabled controls
hidden controls
or
clear helper copy.

==================================================
91. RESPONSIVE / SCROLL BEHAVIOR
==================================================

Even though this task is MOBILE:

design content to scroll naturally.

Do not make fixed-height layouts that break when content grows.

Use sticky elements only where useful:

Bottom Navigation

Save Bar

Primary action in long Full-screen Sheet.

==================================================
92. MICROCOPY
==================================================

Use short, natural Arabic.

Avoid developer terms such as:

RPC
schema
server
V2
atomic
source_type

The Doctor should see simple medical/product language.

==================================================
93. FINAL CONSISTENCY AUDIT
==================================================

Before finishing:

compare every screen against the 5 selected visual reference images.

Ensure:

- same DocGate identity;
- same teal family;
- same cards;
- same button language;
- same top bar;
- same bottom navigation;
- same typography;
- same status presentation;
- same spacing;
- same icon system.

Do not let added screens look like a different product.

==================================================
94. FINAL UX AUDIT
==================================================

Check:

Can a Doctor find today's appointments immediately?

Can he identify a Pending appointment?

Can he Confirm it quickly?

Can he Check-in the patient?

Can he Start and Complete the visit?

Can he reschedule using a real exact Slot?

Can he manage his weekly schedule?

Can he understand a specific date override?

Can he add a holiday?

Can he block only part of a day?

Can he see that schedule conflicts protect existing bookings?

Can he configure Center Confirmation using actual clock time?

Can he find Work Location information?

Can he manage Services & Prices?

Can he understand Patient vs Family beneficiary?

Can he prevent future bookings for one patient?

Can he see operational payment status without confusing it with Finance?

If any answer requires too many taps:

simplify the flow.

==================================================
95. FINAL DELIVERABLE
==================================================

Do not stop after creating only the original 20 screens.

Expand the current prototype into a complete mobile Doctor journey with approximately 45–65 meaningful screens/states.

Reuse existing frames where possible.

Do not duplicate equivalent screens.

Use clear frame names.

Suggested naming:

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

Create clickable prototype connections.

Create clear client demo starting points.

Do NOT build backend.

Do NOT build production code.

The result should feel like:

“A complete DocGate mobile product concept that a real Doctor can explore and understand without explanation.”

Do one final simplification pass after adding the detailed flows.

The final goal is NOT maximum complexity.

The final goal is:

MAXIMUM USEFUL EXPERIENCE
WITH MINIMUM USER CONFUSION.