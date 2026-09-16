UPDATE ONLY THESE 3 PARTS OF THE CURRENT DOCGATE MOBILE PROTOTYPE.

Do NOT redesign the existing prototype.
Do NOT remove other approved screens/features.
Do NOT change the visual identity.

Keep everything else exactly as currently designed.

==================================================
1. NEXT 30 DAYS — SHOW THE FULL CALENDAR GRID
==================================================

Change the mobile “Next 30 Days” Schedule presentation.

DO NOT use the horizontal swipe/date-strip as the main interface.

I want the previous calendar-style presentation where ALL day squares are visible together.

Use a compact 7-column calendar grid showing the complete active Next-30-Days period.

The Doctor should be able to visually compare all upcoming days without horizontal scrolling.

The calendar remains FULLY INTERACTIVE.

Each active day square can be selected.

When selected, show the day details below the calendar:

- date;
- status;
- whether it follows the Weekly Schedule or has a custom override;
- sessions;
- partial blocks;
- booking summary;
- relevant actions.

Keep all agreed date states:

- متاح
- مغلق
- إجازة
- ممتلئ
- غير معد
- انتهت نافذة الحجز — display-only

Selected state must be visually separate from the actual status.

Today must also have its own subtle marker.

If dates before/after the active 30-day range are needed to complete the calendar rows:

show them muted and non-interactive.

The Doctor must still be able from the selected day to:

- تعديل هذا اليوم
- create custom sessions;
- add multiple sessions;
- إغلاق اليوم;
- set Holiday;
- create partial-day block;
- استعادة الجدول الأسبوعي;
- view that day’s bookings;
- save deliberately;
- see conflict protection when existing bookings are affected.

Do not turn the 30-day calendar into a read-only screen.

Keep the relationship clear:

Weekly Schedule
= recurring base

Next 30 Days
= actual upcoming dates

Exact-date Override
= change for one specific date

Restore Weekly
= remove that date-specific change

==================================================
2. FULL ARABIC RTL + FUTURE ENGLISH SUPPORT
==================================================

Correct RTL across the WHOLE APPLICATION.

Arabic RTL must NOT mean only:

“right-align the text.”

When Arabic is active, the entire interface structure must behave as a native RTL application.

This includes:

- overall page flow;
- App Bars;
- Back buttons;
- directional arrows;
- cards;
- forms;
- field icons;
- labels and values;
- tabs;
- segmented controls;
- dropdowns;
- lists;
- Booking rows;
- Work Location cards;
- Schedule rows;
- calendar;
- filter chips;
- menus;
- Bottom Sheets;
- Full-screen Sheets;
- dialogs;
- Bottom Navigation;
- action icon placement.

Directional icons such as Back / Next / Previous / disclosure chevrons must follow RTL correctly.

Non-directional icons such as:

calendar
user
location
clock
medical icons

should not be unnecessarily mirrored.

IMPORTANT:

DocGate must also support English later.

Add a language option:

الإعدادات
→ اللغة

Options:

العربية
English

The design system should be prepared for:

Arabic = RTL
English = LTR

Use Auto Layout and direction-safe reusable components.

BUT:

DO NOT design the English screens now.

DO NOT duplicate the Arabic prototype into English.

We want to save Figma Make quota.

Only prepare the components/layout architecture for future English support.

All visible screens in this task remain Arabic.

==================================================
3. FIRST-TIME DOCTOR MUST START WITH SCHEDULE SETUP
==================================================

Change the post-registration flow for a NEW Doctor.

For a Doctor registering for the FIRST TIME:

do NOT send him directly to the normal Doctor Home Dashboard.

After successful registration:

Create Account
→ WhatsApp OTP Verification
→ Specialty
→ Professional Title
→ Account Ready
→ Schedule Setup

The first important operational task should be:

إعداد الجدول الزمني

Create a simple introductory state:

لنبدأ بإعداد جدولك

Supporting text:

حدد أيام وساعات عملك حتى يتمكن المرضى من معرفة المواعيد المتاحة للحجز.

Primary CTA:

إعداد الجدول الآن

Then enter the Weekly Schedule setup.

If the Doctor already has a usable Work Location:

open Schedule for that Work Location.

If the Doctor has no Work Location yet:

keep him inside the same onboarding journey and add a lightweight step:

أين ستستقبل المرضى؟

Options:

- اختيار منشأة موجودة
- إضافة مكان عمل

After selecting/creating the first Work Location:

continue immediately to Weekly Schedule setup.

During FIRST Schedule setup keep it simple.

Focus only on:

- Saturday through Friday;
- Working / Weekly Off;
- Start Time;
- End Time;
- Consultation Duration;
- multiple Sessions when needed.

Do not initially overwhelm the new Doctor with advanced settings such as:

- Holidays;
- Partial Blocks;
- Conflict Review;
- advanced exact-date Overrides;
- Confirmation Policy;
- Capacity.

After the Doctor saves the first Weekly Schedule:

show:

تم إعداد جدولك بنجاح

Then provide:

Primary:
عرض الأيام الـ30 القادمة

Secondary:
الذهاب إلى الصفحة الرئيسية

If the Doctor chooses:

عرض الأيام الـ30 القادمة

open the full 7-column editable calendar described in modification #1.

IMPORTANT:

This Schedule-first behavior is ONLY for a new Doctor who has not completed initial Schedule setup.

For a returning Doctor who already configured Schedule:

Login
→ Doctor Home

Do NOT send every returning Doctor to Schedule after every login.