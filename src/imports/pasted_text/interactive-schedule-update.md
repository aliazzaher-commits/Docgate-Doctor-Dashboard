IMPORTANT UPDATE — MAKE THE 30-DAY / MONTHLY SCHEDULE FULLY INTERACTIVE AND EDITABLE.

Do NOT treat the Monthly / 30-Day Schedule as a read-only calendar.

This calendar is one of the Doctor’s main operational tools.

Keep all previously approved Schedule logic.

==================================================
1. PURPOSE
==================================================

The Calendar represents the NEXT 30 DAYS.

It may visually look like a monthly calendar,
including adjacent dates needed to complete calendar rows,
but the actual editable scope remains the active Next-30-Days window.

The Doctor must be able to:

- select any active date;
- inspect that date;
- edit only that date;
- close that date;
- mark it as Holiday;
- create custom sessions;
- add a partial-day block;
- restore the Weekly Schedule;
- see existing bookings;
- understand conflicts before saving.

Do NOT turn it into a passive month display.

==================================================
2. ENTRY
==================================================

Work Location
→ Schedule
→

[ الجدول الأسبوعي | الأيام الـ30 القادمة ]

When Doctor selects:

الأيام الـ30 القادمة

open the editable calendar view.

Also allow access through:

عرض التقويم

from the mobile date-strip view.

==================================================
3. CALENDAR LAYOUT
==================================================

Create a clean 7-column calendar.

Semantic weekday order:

السبت
الأحد
الاثنين
الثلاثاء
الأربعاء
الخميس
الجمعة

Respect Arabic RTL naturally.

Show:

current month / month range

Example:

سبتمبر – أكتوبر 2026

If the rolling 30 days cross two months,
show that clearly.

==================================================
4. CALENDAR DATE CELLS
==================================================

Each active date cell must be tappable.

Each cell should show only compact information:

- day number;
- status indicator;
- short status label if space allows;
- optional tiny booking indicator/count;
- selected state.

Do NOT overload each cell with session details.

==================================================
5. DATE STATES
==================================================

Support the approved visual states:

متاح

مغلق

إجازة

ممتلئ

غير معد

Also support the display-only state:

انتهت نافذة الحجز

IMPORTANT:

“انتهت نافذة الحجز” is NOT a replacement for Full.

It appears only when there are theoretically unused Slots,
but none can currently pass the existing booking-window eligibility.

Do not redefine Full.

==================================================
6. SELECTED DATE
==================================================

Selected state must be independent from the original status.

For example:

Holiday + Selected

must still visibly remain Holiday,
with an additional selected outline/highlight.

Do NOT change the status just because the day is selected.

==================================================
7. ADJACENT / OUTSIDE-RANGE DATES
==================================================

To make the grid look like a proper calendar,
you may show dates before/after the active 30-day window.

These dates must be:

- muted;
- visibly secondary;
- non-editable;
- non-mutating.

They exist only for calendar context.

Do NOT expand the actual feature scope beyond the active 30 days.

==================================================
8. TAP A DATE
==================================================

Tapping an active date should update a selected-day panel below the calendar.

Example:

الخميس، 17 سبتمبر 2026

[ متاح ]

Then clearly show one of:

يتبع الجدول الأسبوعي

or

لديه تعديل خاص بهذا اليوم

This distinction is extremely important.

==================================================
9. SELECTED DAY DETAIL
==================================================

Show:

### Status

متاح / مغلق / إجازة / etc.

### Source

يتبع الجدول الأسبوعي

or

تعديل خاص لهذا التاريخ

### Sessions

Example:

08:00 ص – 01:00 م
مدة الاستشارة: 15 دقيقة

05:00 م – 08:00 م
مدة الاستشارة: 30 دقيقة

### Partial blocks

Example:

حظر جزئي
01:30 م – 03:00 م

### Booking summary

Example:

5 حجوزات

3 مواعيد متاحة

Do not derive these counts from unresolved Capacity behavior.

==================================================
10. PRIMARY DAY ACTION
==================================================

Primary action:

تعديل هذا اليوم

This must open an exact-date editor.

The Doctor should never need to edit the weekly recurrence just to change one date.

==================================================
11. EXACT-DATE EDITOR
==================================================

Create a full-screen Sheet:

تعديل الخميس 17 سبتمبر

Important helper:

هذا التعديل يخص هذا التاريخ فقط ولن يغيّر جدول الخميس الأسبوعي.

Available date states:

### يعمل / متاح

Doctor may define custom Sessions.

### مغلق

Close this date only.

### إجازة

Mark this date as Holiday.

Do not confuse Closed and Holiday visually.

==================================================
12. CUSTOM SESSIONS FOR ONE DATE
==================================================

If Doctor chooses a custom working day:

allow multiple sessions.

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

Reuse the SAME Session Editor design used by Weekly Schedule.

Do not build a separate session system.

==================================================
13. SESSION VALIDATION
==================================================

Multiple sessions may not overlap.

Valid:

08:00–13:00

13:00–16:00

Invalid:

08:00–13:00

12:00–15:00

Create an inline error state:

تتداخل هذه الجلسة مع جلسة أخرى.

==================================================
14. SESSION SLOT SUMMARY
==================================================

For each Session,
use Start + End + Consultation Duration.

Example:

08:00–13:00
15 minutes

Show:

عدد المواعيد الممكنة: 20

أول موعد: 08:00 ص

آخر بداية موعد: 12:45 م

IMPORTANT:

13:00 is the end of the Session.

12:45 is the last valid appointment START.

==================================================
15. CAPACITY
==================================================

CAPACITY_PRODUCT_DECISION_REMAINS_DEFERRED.

Do not make Capacity determine which time Slots appear.

Do not implement:

- first N Slots;
- automatic compacting;
- queue sequencing;
- patient priority.

If Capacity is visually preserved,
keep it secondary/non-authoritative.

==================================================
16. CLOSE DATE
==================================================

Allow:

إغلاق اليوم

Show confirmation:

إغلاق الخميس 17 سبتمبر؟

Helper:

لن يكون هذا اليوم متاحًا للحجوزات الجديدة.

IMPORTANT:

Do not say existing bookings will be cancelled.

Existing bookings are protected.

==================================================
17. HOLIDAY
==================================================

Allow:

تعيين كإجازة

Optional:

سبب الإجازة

Then date becomes visually Holiday.

Do not delete existing bookings.

==================================================
18. HOLIDAY RANGE
==================================================

From the calendar Schedule area also provide:

الإجازات والحظر

Then:

إجازة ليوم واحد

إجازة لفترة

For range:

من
إلى

optional reason.

After saving,
all affected active dates should visually update on the calendar.

==================================================
19. PARTIAL-DAY BLOCK
==================================================

Selected date action:

حظر جزء من اليوم

Open Sheet:

حظر جزء من الخميس 17 سبتمبر

From:

01:00 م

To:

03:00 م

Reason optional.

Show preview:

الفترة المحظورة:
01:00 م – 03:00 م

Do not move appointments automatically.

==================================================
20. RESTORE WEEKLY SCHEDULE
==================================================

If selected date has an override,
show:

استعادة الجدول الأسبوعي

Confirmation:

استعادة جدول الخميس الأسبوعي؟

Description:

سيُحذف التعديل الخاص بهذا التاريخ فقط،
وسيعود اليوم إلى الجدول الأسبوعي المعتاد.

Buttons:

إلغاء

استعادة الجدول

This must affect ONLY this date override.

Do not modify all Thursdays.

==================================================
21. VISUAL OVERRIDE INDICATOR
==================================================

Dates with exact-date overrides should have a subtle visual indicator.

Example:

small dot / corner marker / small icon.

Do not create a completely separate status color just for Override.

The actual state remains:

Available / Closed / Holiday / etc.

Override is additional metadata.

==================================================
22. BOOKINGS ON SELECTED DATE
==================================================

Selected Day Details should show a compact Booking section.

Example:

الحجوزات

09:00 ص — محمد عبدالله
10:30 ص — سارة أحمد
12:00 م — خالد سالم

[ عرض جميع حجوزات اليوم ]

Tap this action:

open Work Location Bookings already filtered to that date.

Do not build a duplicate Bookings list inside Schedule.

==================================================
23. SCHEDULE SAVE
==================================================

Do NOT autosave Calendar edits.

After modification show sticky:

لديك تغييرات غير محفوظة

Buttons:

تجاهل

حفظ التغييرات

==================================================
24. LEAVING WITH UNSAVED CHANGES
==================================================

If Doctor navigates away:

لديك تغييرات غير محفوظة

هل تريد مغادرة الصفحة؟

Actions:

البقاء

تجاهل التغييرات

==================================================
25. CONFLICT REVIEW
==================================================

This is mandatory in the monthly-calendar prototype.

If Doctor edits:

working session
Closed
Holiday
Partial Block

and existing bookings conflict with the change:

on Save open:

توجد حجوزات متأثرة

Example:

هذا التغيير يتعارض مع 3 حجوزات موجودة.

Show:

09:30 ص
محمد عبدالله
استشارة عامة

10:00 ص
سارة أحمد
متابعة

10:30 ص
خالد سالم
استشارة تخصصية

Important message:

لن يتم إلغاء أو نقل أي حجز تلقائيًا.

Actions:

عرض الحجوزات المتأثرة

العودة لتعديل الجدول

Do NOT add:

حفظ على أي حال

for an invalid conflicting Schedule change.

==================================================
26. FULL DAY
==================================================

Full is system-derived.

Doctor does NOT manually select:

ممتلئ

as a date override.

If all valid Slots are occupied,
calendar may show:

ممتلئ

The Doctor can still open the date and inspect its sessions/bookings.

==================================================
27. NOT CONFIGURED
==================================================

If a date has no usable weekly configuration:

show:

غير معد

Selected Date Details may say:

لا توجد جلسات مهيأة لهذا اليوم.

CTA:

تهيئة هذا اليوم

This creates an exact-date override,
not a new weekly recurrence unless Doctor explicitly edits Weekly Schedule.

==================================================
28. BOOKING WINDOW ENDED
==================================================

If Slots exist but are no longer eligible for new booking because the current booking window has ended:

show:

انتهت نافذة الحجز

This is display-only.

The Doctor can still inspect the date.

Do not turn it into:

Closed

or:

Full.

==================================================
29. TODAY
==================================================

Today should have its own subtle indicator.

Do not confuse:

Today

with:

Selected.

Example:

small “اليوم” marker.

If today is also selected,
both meanings must remain visually understandable.

==================================================
30. CALENDAR LEGEND
==================================================

Provide compact legend:

● متاح

● مغلق

● إجازة

● ممتلئ

○ غير معد

If needed:

⏱ انتهت نافذة الحجز

Keep selected-state explanation separate.

==================================================
31. QUICK DATE NAVIGATION
==================================================

Provide a small action:

اليوم

to return quickly to today.

Also allow:

Previous / Next month visual navigation

ONLY for viewing the active rolling 30-day context.

Do not accidentally create editable dates outside scope.

==================================================
32. MOBILE UX
==================================================

Although the calendar is editable,
do not make every tiny cell contain action icons.

Interaction should be:

Tap Date
→ Selected Day Details
→ Edit this Day

not:

tiny pencil icon inside every date.

This keeps the calendar clean and touch-friendly.

==================================================
33. CLIENT DEMO FLOW
==================================================

Create clickable flow:

START — Editable 30-Day Schedule

Schedule
→ الأيام الـ30 القادمة
→ calendar
→ select Thursday 17 Sep
→ Selected Day Detail
→ تعديل هذا اليوم
→ add second Session
→ Save
→ updated calendar.

Then another flow:

Calendar
→ select Friday 18 Sep
→ Holiday
→ Save
→ Holiday shown.

Then:

Calendar
→ select Sunday 20 Sep
→ Partial Block
→ Save
→ block shown.

Then:

Calendar
→ select overridden day
→ Restore Weekly
→ confirmation
→ restored state.

==================================================
34. CONFLICT DEMO FLOW
==================================================

Create another clear demo:

Select a day containing bookings
→ إغلاق اليوم
→ Save
→ Conflict Review
→ affected bookings shown
→ return to edit.

This is important for client approval.

==================================================
35. KEEP WEEKLY AND MONTHLY CONNECTED
==================================================

Never present Weekly Schedule and 30-Day Schedule as unrelated systems.

The concept must always be visually clear:

Weekly Schedule
= recurring base.

30-Day Calendar
= real upcoming dates based on that base.

Exact-date override
= exception to one specific date.

Restore Weekly
= remove that exception.

This mental model should be immediately understandable from the UI.

==================================================
36. FINAL CHECK
==================================================

Before finishing verify that the Doctor can:

✓ select an active calendar date
✓ inspect its source/status
✓ edit only that date
✓ add multiple sessions
✓ close date
✓ add one-day Holiday
✓ add Holiday range
✓ add partial-day block
✓ restore Weekly
✓ see bookings for date
✓ navigate to Bookings
✓ see Full as system state
✓ see Not Configured
✓ see Booking Window Ended
✓ save deliberately
✓ see unsaved warning
✓ receive conflict protection
✓ understand that existing bookings are never silently cancelled/moved

Do not simplify the Monthly Calendar into a static display again.