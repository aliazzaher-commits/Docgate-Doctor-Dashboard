Build a complete, high-fidelity MOBILE-FIRST Figma prototype for the Doctor experience of a healthcare platform called:

DocGate

IMPORTANT:
This is a SIDE DESIGN TASK ONLY.

It is completely separate from the existing production implementation.

DO NOT build backend logic.
DO NOT connect APIs.
DO NOT connect Supabase.
DO NOT modify any existing product/code.
DO NOT invent database behavior.

The goal is to create a polished, realistic, clickable Figma prototype that we can present to a doctor/client for approval before development continues.

==================================================
1. PRIMARY VISUAL REFERENCES
==================================================

I have attached 5 reference images.

Use these images as the PRIMARY VISUAL SOURCE OF TRUTH.

Study them carefully before designing.

Match them as closely as practical in:

- overall DocGate visual identity;
- teal / dark turquoise palette;
- white/light backgrounds;
- card shapes;
- input styles;
- shadows;
- border radius;
- mobile spacing;
- visual density;
- icon style;
- typography hierarchy;
- top bars;
- tab bars;
- bottom navigation;
- dashboards;
- lists;
- cards;
- forms;
- calendar presentation;
- sheets;
- buttons;
- status pills.

Do NOT randomly redesign the product into another style.

Do NOT make it look like a generic admin dashboard.

The final prototype should clearly feel like an improved and fully consistent version of the attached DocGate mobile UI references.

However:

THE IMAGES ARE THE VISUAL REFERENCE,
NOT THE FINAL PRODUCT-LOGIC AUTHORITY.

If a label, action, or behavior shown in a generated image conflicts with the product rules below, KEEP THE VISUAL STYLE but use the product rule described in this prompt.

==================================================
2. DESIGN GOAL
==================================================

The product should feel:

- extremely easy to understand;
- calm;
- professional;
- medical;
- modern;
- premium but not luxurious;
- trustworthy;
- fast to scan;
- touch-friendly;
- Arabic-first;
- suitable for doctors who are not technical users.

Avoid:

- clutter;
- oversized cards;
- unnecessary decoration;
- excessive gradients;
- tiny touch targets;
- deep navigation;
- repeated information;
- too many buttons visible at once;
- forms that feel bureaucratic.

The doctor should usually know:

1. Where am I?
2. What needs my attention?
3. What is the next action?

within a few seconds.

==================================================
3. LANGUAGE AND DIRECTION
==================================================

Primary prototype language:

Arabic.

Use proper RTL layout.

All Arabic alignment, arrows, tab order, icons, sheets and navigation must feel naturally RTL.

Use realistic Arabic medical/product language.

Recommended Arabic typography style:

Cairo / IBM Plex Sans Arabic / similarly clean Arabic UI font.

English may appear only where naturally useful:

DocGate
Email examples
professional English doctor name
medical abbreviations such as ECG

Prepare the design structure so an English LTR version could later be derived easily.

==================================================
4. FIGMA DESIGN SYSTEM
==================================================

Before creating all screens, establish a reusable mini design system.

Create reusable components for:

- Primary Button
- Secondary Button
- Destructive Button
- Text Input
- Password Input
- Phone Input
- OTP Digit Input
- Search Field
- Select / Dropdown
- Time Input
- Date Item
- Status Badge
- Stat Card
- Booking Row
- Work Location Card
- Session Row
- Setting Row
- Toggle
- Tab
- Segmented Control
- Bottom Navigation
- Top App Bar
- Empty State
- Alert / Helper Box
- Modal
- Bottom Sheet
- Full-screen Sheet
- Toast / success feedback
- Skeleton/loading placeholder

Use Auto Layout properly.

Use consistent spacing tokens.

Suggested spacing rhythm:

4
8
12
16
20
24
32

Use one consistent radius system.

Keep controls comfortably touchable.

==================================================
5. COLOR DIRECTION
==================================================

Use the attached references as the exact visual inspiration.

Primary:
deep DocGate teal / dark turquoise.

Secondary:
lighter teal / mint.

Surfaces:
white,
very light neutral gray,
subtle mint-tinted backgrounds where useful.

Semantic states:

Available / Success:
soft green.

Pending:
soft amber.

Cancelled / Error:
soft red.

Information:
soft blue.

Inactive / not configured:
neutral gray.

Avoid using bright saturated colors unnecessarily.

Color must never be the only status indicator.
Also use text/icon/badge.

==================================================
6. PROTOTYPE STRUCTURE
==================================================

Organize the Figma file into clear pages/sections:

01 — Foundations
02 — Components
03 — Authentication
04 — Doctor Home
05 — Profile
06 — Work Locations
07 — Schedule
08 — Bookings
09 — Patient Controls
10 — Finance
11 — Prototype Flow

Create a clear Flow Map.

The client should be able to understand the Doctor journey from:

Welcome
→ Login / Registration
→ First entry
→ Doctor Home
→ Profile
→ Work Locations
→ Schedule
→ Bookings
→ Patient-related controls
→ Finance

==================================================
7. MOBILE FRAME
==================================================

Use a modern standard mobile frame approximately:

390 × 844

or an equivalent modern iPhone frame.

Do not design primarily for the device chrome.

The UI itself is the priority.

Use the attached phone references for visual proportions.

==================================================
8. AUTHENTICATION FLOW
==================================================

Follow the simplicity of the attached references and the Vezeeta-inspired flow.

The goal is:

VERY EASY REGISTRATION.

Do not make the user complete the full professional verification process before seeing the Doctor workspace.

Create these states/screens.

--------------------------------------------------
A. Welcome / Splash
--------------------------------------------------

Use the reference styling.

Include:

DocGate logo
short professional tagline

Primary:
تسجيل الدخول

Secondary:
إنشاء حساب جديد

Optional:
استكشاف التطبيق

Keep this screen extremely clean.

--------------------------------------------------
B. Login
--------------------------------------------------

Use segmented control:

رقم الهاتف
البريد الإلكتروني

Phone login:

country code
phone number
password

Email login:

email
password

Include:

نسيت كلمة المرور؟

Primary:
تسجيل الدخول

Secondary link:
إنشاء حساب جديد

Do not expose technical authentication terms.

--------------------------------------------------
C. Create Account
--------------------------------------------------

Fields:

الاسم الكامل

الدولة / مفتاح الدولة

رقم الهاتف

البريد الإلكتروني

كلمة المرور

تأكيد كلمة المرور

Primary:
إنشاء الحساب / متابعة

Keep visual validation simple.

--------------------------------------------------
D. WhatsApp OTP
--------------------------------------------------

6-digit OTP.

Text such as:

تم إرسال رمز التحقق إلى رقمك عبر واتساب

Masked phone number.

Countdown.

إعادة إرسال الرمز

تغيير رقم الهاتف

After correct OTP, transition immediately.

Do not create a long verification experience.

--------------------------------------------------
E. Specialty & Professional Title
--------------------------------------------------

This is IMPORTANT even if it is not prominent in one of the reference boards.

After phone verification, ask for:

التخصص الطبي

المسمى المهني

Examples:

طبيب عام
أخصائي
استشاري

Use searchable selectors.

Keep the screen short.

--------------------------------------------------
F. First Entry
--------------------------------------------------

Doctor must be able to enter DocGate quickly.

DO NOT force completion of:

- medical license;
- certificates;
- identity documents;
- complete professional profile;
- payment;

before allowing Doctor to see the workspace.

After the essential registration steps:

enter Doctor Home.

==================================================
9. PROFESSIONAL PROFILE COMPLETION
==================================================

After entering DocGate, show a clear progress/checklist flow.

Use the reference image style.

Example:

أكمل ملفك الشخصي

20% / 40% / 80%

Checklist:

المعلومات الأساسية
المعلومات المهنية
التخصص
الترخيص الطبي
المؤهلات والشهادات
الخبرات العملية
مواقع العمل
التحقق من الهوية

Allow:

إكمال الآن
إكمال لاحقًا

Verification is important for public publication and trust,
but should not prevent the Doctor from exploring his workspace.

==================================================
10. PAYMENT DURING ONBOARDING
==================================================

DO NOT make payment mandatory.

Do not copy Vezeeta’s mandatory payment wall.

If a plan/payment concept is shown during the prototype:

show:

اختيار الخطة

and provide a very clear:

تخطي الآن

The Doctor must still enter the workspace.

Do not make this a primary part of the first approval prototype unless needed.

==================================================
11. DOCTOR MOBILE HOME
==================================================

Use the attached reference Home as a strong visual starting point.

Make it useful, not decorative.

Header:

مرحبًا د. أحمد

small avatar

notifications.

Show important today summary.

Example:

مواعيد اليوم
مرضى اليوم
طلبات تحتاج تأكيد
الجلسات المكتملة

Then:

المواعيد القادمة

show 2–3 upcoming bookings.

Then:

إجراءات سريعة

Possible quick actions:

الحجوزات
إدارة الجدول
مواقع العمل
الملف الشخصي

Then:

Profile Completion Card.

Then:

important notifications/tasks.

Do not create an extremely long homepage.

==================================================
12. GLOBAL MOBILE NAVIGATION
==================================================

Make navigation consistent across authenticated Doctor screens.

Recommended bottom navigation:

الرئيسية
الحجوزات
المرضى
الرسائل
المزيد

Do not randomly change the bottom-nav structure screen by screen.

Work Locations,
Schedule,
Services,
Finance

can be reached naturally through the Doctor workspace / More / contextual screens.

Use no more than 5 bottom navigation items.

==================================================
13. DOCTOR PROFILE
==================================================

Follow the reference.

Show:

profile image
Arabic name
English name if available
professional title
specialty
license information
bio
languages
education
qualifications
experience
certificates

Use clean sections.

Editing can open:

full-screen Sheet
or dedicated Edit screen.

Do not overload the profile overview.

==================================================
14. WORK LOCATIONS
==================================================

Create:

Work Locations List

Each card may show:

location name
facility type
city/area
verification/trust state
active/inactive state
short useful summary

Primary action:

إضافة مكان عمل جديد

Then:

Work Location Details.

Use a clean location header.

The Work Location feature order must respect:

Overview
Location Information
Schedule
Services & Prices
Bookings
Payment

IMPORTANT RELATIVE ORDER:

Schedule
→ Services & Prices
→ Bookings
→ Payment

Bookings must be immediately before Payment.

==================================================
15. WORK LOCATION OVERVIEW
==================================================

Use the attached reference.

Possible summary:

appointments this month
patient count
clinic/service count
rating if actually relevant
location information
address
working hours
contact

Do not invent major new analytics.

==================================================
16. MOBILE WEEKLY SCHEDULE
==================================================

The mobile weekly schedule must be compact.

DO NOT use large tall square cards for every weekday.

Use compact tappable rows.

Example:

السبت                         يعمل >
08:00–13:00 · جلسة واحدة

الأحد                         يعمل >
فترتان

الجمعة               إجازة أسبوعية >

Rows should be easy to scan.

Opening a day goes to the existing style of mobile editor / Sheet.

==================================================
17. 30-DAY SCHEDULE
==================================================

Use the attached references for visual inspiration.

For mobile, prioritize ease of use.

Preferred primary interaction:

horizontal day/date selector
+
selected-day detail.

A monthly calendar may be available as a clear secondary calendar view if visually useful in the prototype.

Do NOT make the Doctor interact with tiny calendar cells as the only method.

Status states:

متاح
مغلق
إجازة
ممتلئ
غير معد

Selected state is visually separate from the original day status.

==================================================
18. SESSION EDITOR
==================================================

Use a Full-screen Sheet or dedicated mobile form.

Fields:

اسم الجلسة — optional

وقت البداية

مدة الاستشارة

وقت النهاية

Session Capacity may appear visually because it is an existing product concept,
BUT its booking-distribution behavior is still NOT approved.

Do not make Capacity determine any visible patient slot behavior in this prototype.

If useful add a subtle annotation in the design documentation:

Capacity distribution logic pending product approval.

Show computed summary.

Example:

08:00–13:00

مدة الاستشارة: 15 دقيقة

أول موعد: 08:00

آخر بداية موعد: 12:45

IMPORTANT:

The last Slot is the last valid appointment START time.

==================================================
19. HOLIDAYS / BLOCKS
==================================================

Create a simple UI supporting:

إجازة ليوم واحد

إجازة لفترة

حظر جزئي خلال اليوم

optional reason.

Keep management clear and compact.

==================================================
20. BOOKING CONFIRMATION POLICY
==================================================

IMPORTANT:

Do NOT use the old:

30 minutes
60 minutes
90 minutes
120 minutes

model.

Do NOT use the incorrect relative-time settings shown in some generated examples.

Use the approved actual-clock-time model.

Options:

تأكيد فوري

تأكيد في المركز

When Confirm At Center is selected:

وقت تأكيد الحجز في المركز

Options:

في أي وقت قبل الموعد

في وقت محدد

خلال فترة زمنية

Specific time example:

09:00 ص

Time range example:

من 08:00 ص
إلى 10:00 ص

Use actual local clock-time inputs.

DO NOT include mandatory automatic cancellation when the confirmation window expires.

That remains a separate future decision.

==================================================
21. SERVICES & PRICES
==================================================

Create a simple Work Location section for:

services
consultation types
prices
duration

Keep it visually consistent.

Do not design a huge service management system.

This tab exists between Schedule and Bookings.

==================================================
22. WORK LOCATION BOOKINGS
==================================================

Follow the attached Bookings reference closely but improve hierarchy.

Use:

horizontal date strip

selected date

compact counters

search

status filter

dense booking list.

Statuses may include:

قيد الانتظار
مؤكد
مكتمل
ملغي
لم يحضر

Do not show every possible button on each row.

Booking row should prioritize:

appointment time
patient
service
status
payment information
current next action.

Tapping opens Booking Details.

==================================================
23. BOOKING DETAILS
==================================================

Use Full-screen Sheet on mobile.

Display:

patient identity
actual beneficiary if family booking
phone/contact where allowed
booking date
exact booking time
service
duration
Work Location
booking status
payment status
patient-provided note
internal operational note

Then one clear:

Primary Next Action.

Possible state-driven actions:

Confirm
Check-in
Start Visit
Complete
No-show

depending on state.

Secondary actions:

Reschedule
Cancel
Reminder
Edit note

Do not show actions that do not make sense for the current booking state.

==================================================
24. RESCHEDULE
==================================================

Patient keeps an exact appointment time.

Show:

current appointment

select a date

available exact Slots

select one Slot

Confirm Reschedule.

Do NOT represent rescheduling as a free-form arbitrary datetime input.

==================================================
25. PATIENT SETTINGS / RESTRICTIONS
==================================================

Keep these accepted concepts.

--------------------------------------------------
Automatic confirmation
--------------------------------------------------

Arabic:

تأكيد الحجوزات القادمة تلقائيًا

Only visually show it when it makes logical sense.

If Work Location is already Instant Confirmation:

the option is redundant and can be hidden.

If confirmation is a hard Provider requirement:

do not imply Doctor can override it.

--------------------------------------------------
No prepayment
--------------------------------------------------

Arabic:

السماح بالحجز بدون دفع مسبق

Keep this product capability.

But do not show a meaningless toggle when this Work Location already uses Pay at Visit.

Only display when it actually represents a valid exception.

--------------------------------------------------
Blocking
--------------------------------------------------

Use:

منع الحجوزات المستقبلية

Description should make clear:

blocks NEW future bookings with this Doctor.

It does NOT cancel existing appointments.

Add optional internal reason.

Keep blocking as a rare/destructive action.

Do not make it a primary everyday setting.

==================================================
26. FAMILY MEMBER VISUAL SUPPORT
==================================================

Bookings may be:

for the account owner
or
for a family member.

Where relevant, clearly show:

المريض
or
المستفيد

Example:

الحجز لـ:
سارة أحمد — ابنة المريض

Do not confuse account owner with actual care recipient.

==================================================
27. REMINDERS
==================================================

Manual reminder may be shown:

إرسال تذكير

Do not design automatic notification scheduling settings as if they are already finalized.

Automatic location notification configuration remains deferred.

==================================================
28. EMERGENCY ACTION
==================================================

If Emergency Actions appear:

do not invent a second emergency booking engine.

Make it visually lead to Schedule management.

Example:

إجراء طارئ
→ تعديل الجدول
→ إغلاق اليوم / حظر فترة

Do not automatically cancel bookings in the prototype.

==================================================
29. FINANCE / PAYMENT
==================================================

Use the attached Finance reference visually.

Show operational summary such as:

الرصيد
الإيرادات
المعاملات
المستحقات

Payment status may be visible in Booking details.

Do not imply that the Bookings section manages:

refund processing
settlement
provider payouts

Those belong in Finance.

==================================================
30. STRICTLY DO NOT ADD
==================================================

Do not add:

VIP patient system

Waitlist

queue-only booking

public Walk-in

automatic patient priority

Ramadan scheduling system

appointment buffer system

Copy Week

advanced Capacity behavior

new payment gateway workflow

large Patient CRM

new automatic notification engine

mandatory subscription/payment wall

==================================================
31. STATUS & FEEDBACK UX
==================================================

Design all important screens with realistic UI states where helpful:

default
selected
disabled
loading
empty
success
error

For example:

No bookings today

No Work Locations

No available Slots

Profile incomplete

Action success Toast.

Do not leave prototype only with perfect happy-state screens.

==================================================
32. MOBILE SHEET BEHAVIOR
==================================================

Use bottom/full-screen Sheets where appropriate.

Examples:

filter
session editor
booking details
edit patient exception
block patient confirmation
time picker

On mobile:

major/detail editors should usually be full-screen Sheets.

Small filters may be Bottom Sheets.

==================================================
33. ACCESSIBILITY
==================================================

Make controls readable.

Minimum practical touch target:
approximately 44px.

Use good contrast.

Do not depend only on color.

Use clear visible selected state.

Keep field labels visible.

Do not rely only on placeholders.

==================================================
34. PROTOTYPE INTERACTIONS
==================================================

Create realistic clickable prototype navigation.

At minimum wire:

Welcome
→ Login

Welcome
→ Create Account

Create Account
→ OTP

OTP
→ Specialty

Specialty
→ Doctor Home

Doctor Home
→ Complete Profile

Doctor Home
→ Work Locations

Work Locations
→ Work Location

Work Location
→ Schedule

Schedule
→ Session Editor

Schedule
→ Holiday / Block

Work Location
→ Services & Prices

Work Location
→ Bookings

Bookings
→ Booking Details

Booking Details
→ Reschedule

Booking Details
→ Patient Settings

Work Location
→ Payment

Also connect bottom navigation consistently.

==================================================
35. TRANSITIONS
==================================================

Use simple professional transitions:

Smart Animate
200–300ms

Sheets:
slide up

Page transitions:
subtle horizontal navigation

Avoid flashy animation.

==================================================
36. VISUAL CONSISTENCY AUDIT
==================================================

Before completing, inspect all screens together.

Make sure:

same button style
same header height
same cards
same typography scale
same radius
same status badge language
same bottom navigation
same icon family
same spacing
same teal colors

Do not let each screen look like a different app.

==================================================
37. IMPORTANT PRODUCT DECISIONS TO PRESERVE
==================================================

Do not accidentally contradict these:

- exact appointment Slot booking remains the core booking model;
- patient chooses exact appointment time;
- Schedule V2 concept remains exact-time based;
- Capacity booking-distribution behavior is still unresolved;
- Provider restrictions cannot be visually bypassed by Doctor;
- patient block affects only future bookings;
- blocking does not cancel existing appointments;
- patient no-prepayment exception is conditional;
- patient auto-confirm is conditional;
- Finance remains separate from Booking operations;
- Work Location Bookings belong to that Work Location only;
- Booking confirmation at center uses actual clock times;
- no forced payment during initial Doctor registration;
- professional verification may be completed after first entry;
- WhatsApp OTP remains part of registration.

==================================================
38. REFERENCE ADHERENCE
==================================================

This is very important.

Do not ignore the attached screenshots.

They are the selected presentation direction.

Try to preserve:

- the clean DocGate teal header style;
- large white content surfaces;
- simple thin borders;
- mobile card structure;
- the dashboard structure;
- Work Location cards;
- Schedule form structure;
- Booking list density;
- Finance summary styling;
- phone proportions;
- icon treatment.

Improve usability where necessary,
but do NOT create a completely different visual system.

Aim for:

“the same design direction, refined into a consistent professional product.”

==================================================
39. FINAL DELIVERABLE
==================================================

Create a polished Figma prototype suitable for a client presentation.

It should contain:

- foundations/styles;
- reusable components;
- complete mobile screen flow;
- Arabic RTL screens;
- clickable prototype;
- realistic content;
- organized frame names;
- clear grouping;
- no backend;
- no code;
- no API implementation.

Use clear frame names such as:

MOB-01-Welcome
MOB-02-Login
MOB-03-CreateAccount
MOB-04-OTP
MOB-05-Specialty
MOB-06-Home
MOB-07-ProfileChecklist
MOB-08-DoctorProfile
MOB-09-WorkLocations
MOB-10-WorkLocationOverview
MOB-11-WeeklySchedule
MOB-12-30DaySchedule
MOB-13-SessionEditor
MOB-14-HolidayBlock
MOB-15-ConfirmationPolicy
MOB-16-ServicesPrices
MOB-17-Bookings
MOB-18-BookingDetails
MOB-19-Reschedule
MOB-20-PatientControls
MOB-21-Finance

You may add small necessary supporting states/overlays,
but do NOT expand product scope.

Before finishing, do one final UX pass asking:

“Can a Doctor understand and use this screen immediately without training?”

If not, simplify it.