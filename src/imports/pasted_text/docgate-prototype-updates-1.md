UPDATE THE CURRENT DOCGATE MOBILE PROTOTYPE WITH THE FOLLOWING INFORMATION-ARCHITECTURE AND SCHEDULE CHANGES.

DO NOT restart the design.
DO NOT redesign the approved visual identity.
DO NOT remove unrelated approved features.
DO NOT create backend logic.

This is a refinement of the CURRENT prototype.

The main goal is now:

- reduce duplicated navigation;
- make “Appointments / المواعيد” the Doctor’s central daily workspace;
- keep Schedule + Bookings + Booking Confirmation close together;
- keep Work Locations lighter;
- make Home reflect the Doctor’s real daily shifts across locations;
- preserve all previously approved Schedule logic.

==================================================
1. MONTHLY / NEXT-30-DAYS SCHEDULE
==================================================

KEEP THE CURRENT MONTHLY / 30-DAY CALENDAR VISUAL DESIGN EXACTLY AS IT IS.

Its current visual direction is approved.

Do NOT replace it with horizontal scrolling.

Do NOT redesign the calendar cells.

Only ADD any previously approved Schedule capabilities that are still missing.

The Monthly / Next-30-Days calendar must support:

- full visible 7-column calendar grid;
- available dates;
- closed dates;
- holidays;
- full dates;
- not configured dates;
- booking-window-ended display state;
- Today marker;
- Selected marker;
- exact-date Override marker;
- selected-day details;
- multiple sessions on one exact date;
- edit exact date;
- close exact date;
- one-day Holiday;
- Holiday range;
- partial-day block;
- Restore Weekly Schedule;
- bookings summary for selected date;
- deliberate Save;
- Unsaved Changes warning;
- Schedule Conflict Review;
- existing bookings must never silently move/cancel.

Keep:

Weekly Schedule
= recurring base.

Monthly / 30 Days
= actual upcoming dates.

Exact-date Override
= special change for one date.

Restore Weekly
= remove that one-date override.

==================================================
2. BOOKING CONFIRMATION MUST ALSO BE ACCESSIBLE
==================================================

The approved booking confirmation policy must remain part of the Doctor’s operational scheduling experience.

It must support:

### تأكيد فوري

No extra timing configuration.

### تأكيد في المركز

Then choose ONE of:

- في أي وقت قبل الموعد
- في وقت محدد
- خلال فترة زمنية

For specific time:

example:
09:00 ص

For time range:

من 08:00 ص
إلى 10:00 ص

DO NOT use:

30 / 60 / 90 / 120 minutes

or:

6 hours / 24 hours

Do NOT add automatic cancellation after the confirmation window.

==================================================
3. WEEKLY SCHEDULE — KEEP FEATURES, REFINE VISUAL DESIGN
==================================================

KEEP all current Weekly Schedule functionality.

Do NOT replace its product logic.

However, improve the MOBILE visual presentation using the attached client reference video as VISUAL inspiration.

The video is a Desktop concept.

DO NOT copy the Desktop layout literally.

Adapt its strongest visual ideas into a clean mobile interface.

==================================================
4. WEEKLY SCHEDULE — VISUAL IDEAS TO BORROW
==================================================

From the client reference video, use these approved ideas:

### A. Clear day cards

Each weekday should feel like a compact operational card.

Example:

الخميس
يعمل

[ صباحي ]
08:00 ص – 01:00 م
15 دقيقة
20 موعدًا ممكنًا

[ مسائي ]
05:00 م – 08:00 م
30 دقيقة
6 مواعيد ممكنة

[ + إضافة فترة ]

Keep the mobile card compact.

Do not use huge day cards.

### B. Visual session distinction

Allow optional session names such as:

صباحي
مسائي
عيادة متابعة

Use subtle tinted session blocks inspired by the client video.

Do not use excessive colors.

### C. Weekly Off selector

Provide a quick, clear way to define:

الإجازة الأسبوعية

Example compact chips:

السبت
الأحد
الاثنين
الثلاثاء
الأربعاء
الخميس
الجمعة

Selected Weekly Off days should be immediately understandable.

This still maps to the existing:

Working / Weekly Off

logic.

### D. Appointment summary

For each Session, show a useful summary derived ONLY from:

Start
End
Consultation Duration.

Example:

08:00–13:00
15 دقيقة
20 موعدًا ممكنًا

Do NOT derive this number from Capacity.

### E. Add/Edit period

Tapping a Session should open the existing style of Full-screen Sheet.

Fields:

اسم الفترة — اختياري

وقت البداية

وقت النهاية

مدة الاستشارة

Computed summary.

Actions:

حفظ

حذف الفترة

Do not introduce unrelated settings inside the Session editor.

==================================================
5. DO NOT COPY THESE CLIENT-VIDEO FEATURES
==================================================

The reference video contains concepts that are NOT currently approved.

DO NOT add:

VIP

VIP Slot allocation

special VIP booking behavior

custom weekly recurrence ending on a date

repeat for N weeks

new “electronic booking enabled” switch per Session

different booking method per Session

duplicate booking-confirmation controls inside every Session

Copy Week

Capacity-based Slot distribution

queue behavior.

Use the video for presentation inspiration ONLY.

==================================================
6. CURRENT WEEKLY PRODUCT LOGIC REMAINS
==================================================

Weekly Schedule still supports:

Saturday → Friday

Working / Weekly Off

multiple Sessions/day

adjacent Sessions allowed:

08:00–13:00
13:00–16:00

overlapping Sessions forbidden:

08:00–13:00
12:00–15:00

Start

End

Consultation Duration

last valid Slot START.

Example:

08:00–13:00
15 minutes

last appointment start:

12:45

NOT:

13:00.

CAPACITY_PRODUCT_DECISION_REMAINS_DEFERRED.

==================================================
7. HOME — REPLACE SINGLE NEXT-APPOINTMENT CARD WITH SHIFT GROUPING
==================================================

The current green “Next Appointment” card should become smarter.

The Doctor may work at MULTIPLE locations during the same day.

Example:

Tomorrow morning:
برج الأطباء

Tomorrow afternoon:
مركز المدينة الطبي

The Home should reflect that operational reality.

Instead of showing only ONE isolated appointment card,
group upcoming appointments by WORK SHIFT / WORK LOCATION.

==================================================
8. HOME — UPCOMING WORK SHIFTS
==================================================

Create a section such as:

جدولك القادم

or:

دوامك القادم

Example:

--------------------------------
برج الأطباء
غدًا · الفترة الصباحية
08:00 ص – 01:00 م
[ location color/accent ]

3 مرضى

09:00 ص — محمد عبدالله
09:30 ص — سارة أحمد
10:30 ص — خالد سالم

[ عرض حجوزات برج الأطباء ]
--------------------------------

Then directly below:

--------------------------------
مركز المدينة الطبي
غدًا · الفترة المسائية
04:00 م – 08:00 م
[ different subtle accent ]

4 مرضى

04:30 م — نورة علي
05:00 م — أحمد محمد
...

[ عرض حجوزات مركز المدينة ]
--------------------------------

==================================================
9. HOME SHIFT CARD DESIGN
==================================================

Each Work Shift Card should prioritize:

Work Location

day/date

Morning / Afternoon / Evening label where useful

session time

number of patients

patient rows ordered by exact appointment time.

Use subtle visual color differentiation between Work Locations.

Do NOT use random bright colors.

Colors identify location/shift visually,
not medical severity.

Keep cards elegant and readable.

==================================================
10. HOME PATIENT ROWS
==================================================

Inside each shift card:

RIGHT:
patient icon + patient name / details

LEFT:
status + navigation arrow where relevant.

Respect the recently corrected RTL card structure.

Do not reintroduce:

Name far left
Status next to icon

problem.

==================================================
11. HOME CARD EXPANSION
==================================================

Do not show 10 patients inside one Home card.

Show approximately:

2–4 upcoming patients.

Then:

عرض كل المواعيد

which opens Appointments already scoped to that Work Location.

==================================================
12. REMOVE SCHEDULE + BOOKINGS FROM WORK LOCATION WORKSPACE
==================================================

We are simplifying navigation.

Inside Work Location Details / Workspace:

REMOVE duplicated direct tabs for:

الجدول الزمني

الحجوزات

These features will now be centrally managed through:

المواعيد

in the main footer.

Do NOT delete their functionality.

Only move their PRIMARY navigation location.

==================================================
13. FIRST-TIME SCHEDULE SETUP REMAINS
==================================================

For a newly registered Doctor:

Registration
→ WhatsApp Verification
→ Specialty
→ Professional Title
→ Schedule Setup

still remains.

That onboarding Schedule setup stays exactly as previously approved.

After initial setup,
ongoing Schedule + Booking management happens mainly through:

المواعيد

in Bottom Navigation.

==================================================
14. APPOINTMENTS BECOMES THE CENTRAL OPERATIONAL HUB
==================================================

Create one central screen:

المواعيد

accessible directly from Bottom Navigation.

This becomes the Doctor’s primary operational workspace.

==================================================
15. WORK LOCATION SWIPE TABS
==================================================

At the TOP of the Appointments screen,
add horizontally swipeable Work Location / Channel tabs.

Arabic RTL.

Example:

[ مركز المدينة ]
[ برج الأطباء ]
[ مستشفى الجمهورية ]
[ أونلاين ]
[ عيادتي الخاصة ]

The Doctor can swipe horizontally between locations.

Selected location should be very clear.

Do not use giant tabs.

Use compact chips/cards.

==================================================
16. EACH LOCATION HAS ITS OWN DATA
==================================================

When Doctor changes selected Work Location:

Bookings

Weekly Schedule

Next 30 Days

Booking Confirmation Policy

must all update to that location/channel.

The Doctor should always understand:

“Which location am I currently managing?”

Keep the selected Work Location visible.

==================================================
17. APPOINTMENTS INTERNAL NAVIGATION
==================================================

Inside the selected Work Location in “المواعيد”,
use a simple secondary navigation.

Recommended:

[ الحجوزات | الجدول | سياسة الحجز ]

Keep it compact.

==================================================
18. BOOKINGS SUBTAB
==================================================

الحجوزات

contains the existing approved Bookings workspace:

date navigation

counters

search

filters

active filter chips

booking list

booking details

confirm

check-in

start visit

complete

cancel

no-show

manual reminder

exact-Slot reschedule

Family Member beneficiary

Provider restrictions.

Do not duplicate another booking screen elsewhere.

==================================================
19. SCHEDULE SUBTAB
==================================================

Inside:

الجدول

show:

[ الجدول الأسبوعي | الأيام الـ30 القادمة ]

Weekly uses the refined mobile cards described above.

30 Days uses the CURRENT approved full calendar grid.

Do not create another Schedule location elsewhere.

==================================================
20. BOOKING POLICY SUBTAB
==================================================

Inside:

سياسة الحجز

show the booking confirmation configuration for the SELECTED Work Location.

Options:

تأكيد فوري

تأكيد في المركز

If Confirm At Center:

في أي وقت قبل الموعد

في وقت محدد

خلال فترة زمنية.

This is NOT a generic Settings screen anymore.

It belongs operationally with:

Appointments + Schedule

for each location.

==================================================
21. REMOVE CONFIRMATION POLICY FROM GENERIC SETTINGS
==================================================

Do not repeat:

Instant Confirmation

Confirm At Center

inside generic application Settings.

Its primary place is now:

المواعيد
→ selected Work Location
→ سياسة الحجز

One canonical UI location.

Reduce duplication.

==================================================
22. SERVICES TAB — CONDITIONAL BY WORK LOCATION TYPE
==================================================

Remove:

الخدمات والأسعار

from hospital/provider Work Location workspace.

For Provider/Hospital locations:

the Doctor should NOT manage hospital services through his personal workspace.

Do not show that management tab.

==================================================
23. SERVICES REMAIN FOR DIRECT DOCTOR CHANNELS
==================================================

Services & Prices remains available ONLY where it makes sense for Doctor-controlled channels, such as:

أونلاين

عيادة خاصة

For these channel types the Doctor may manage:

service name

duration

price

active state

using Yemeni Rial.

Do not remove Services globally.

Make the tab conditional.

==================================================
24. BOTTOM NAVIGATION — MOVE PATIENTS OUT
==================================================

Remove:

المرضى

from Bottom Navigation.

Move Patient access into:

المزيد

Do not delete Patients functionality.

Only change navigation priority.

==================================================
25. ADD APPOINTMENTS TO BOTTOM NAVIGATION
==================================================

Ensure:

المواعيد

is directly available in Bottom Navigation.

There must be only ONE main Appointments item.

Do not accidentally create duplicate:

المواعيد

or:

الحجوزات

footer destinations.

Appointments is the unified operational hub.

Preserve the other currently approved footer items.

==================================================
26. MORE MENU — PATIENTS
==================================================

Inside:

المزيد

add:

المرضى

This opens the existing Patients area.

Do not make Patient CRM more complex.

==================================================
27. UNIFY PROFILE + PROFILE COMPLETION
==================================================

Currently:

الملف الشخصي

and:

إكمال الملف الشخصي

feel duplicated.

Merge them into ONE coherent Doctor Profile experience.

==================================================
28. NEW PROFILE STRUCTURE
==================================================

When Doctor opens:

الملف الشخصي

show the normal profile header:

photo

name

professional title

specialty

verification state.

Immediately below show:

نسبة اكتمال الملف

Example:

75%

with the existing progress/loading style.

Then:

أكمل ملفك المهني

with incomplete sections.

==================================================
29. PROFILE CONTENT — ONE PLACE
==================================================

Inside the same Profile screen,
organize all editable information.

Use one clear tab/segmented system such as:

[ الأساسية | المهنية | المؤهلات والوثائق | الخبرات ]

or another simple equivalent.

Do not require Doctor to jump between:

Profile

Profile Completion

Professional Information

Qualifications

Certificates

Experience

as independent More-menu entries.

They all belong to the unified Profile.

==================================================
30. PROFILE COMPLETION
==================================================

Each incomplete profile item remains directly editable.

Example:

المؤهلات العلمية
80%

Tap

→ Qualifications list

→ Add/Edit

→ Save

→ return to Profile

→ progress updates.

Keep all previously approved editable features.

==================================================
31. CLEAN “MORE” MENU
==================================================

Because Profile is now unified,
remove duplicate entries such as separate:

المعلومات الأساسية

المعلومات المهنية

المؤهلات

الشهادات

الخبرات

if they currently appear as top-level More items.

Replace them with ONE:

الملف الشخصي

entry.

==================================================
32. REMOVE DUPLICATE SCHEDULE MENU ENTRIES
==================================================

Remove top-level More / Settings entries for:

الجدول الأسبوعي

الجدول الشهري / 30 يوم

because Schedule is now managed through:

Bottom Navigation
→ المواعيد
→ selected Work Location
→ الجدول.

Do not remove Schedule functionality.

Only remove duplicate navigation.

==================================================
33. REMOVE DUPLICATE SERVICES MENU ENTRY
==================================================

Remove generic top-level:

الخدمات والأسعار

from More / Settings.

Services management appears only contextually for:

Online

Private Clinic

where the Doctor controls the channel.

==================================================
34. KEEP WORK LOCATIONS
==================================================

Keep:

مواقع العمل

inside More / management area.

This remains where Doctor manages:

location identity

address

verification

relationship

contact information

etc.

But NOT operational Schedule/Bookings.

==================================================
35. KEEP FINANCE — IMPROVE LOCATION NAVIGATION
==================================================

Keep:

المالية والمدفوعات

as currently designed.

Do not move Finance into Appointments.

However, inside Finance add the SAME style of compact Work Location swipe tabs at the top.

Example:

[ كل المواقع ]
[ مركز المدينة ]
[ برج الأطباء ]
[ مستشفى الجمهورية ]
[ أونلاين ]

==================================================
36. FINANCE LOCATION FILTER
==================================================

Default may be:

كل المواقع

Then selecting a Work Location updates:

Overview

Transactions

Payment Settings / eligibility

for that specific location.

This makes Finance easy without creating separate Finance pages per hospital.

==================================================
37. FINANCE MUST REMAIN REALISTIC
==================================================

Keep previously approved:

نظرة عامة

المعاملات

إعدادات الدفع

period filter

payment status

payment method

transaction details

Yemeni Rial.

Do not add Gateway configuration.

==================================================
38. IMPORTANT NO-DUPLICATION RULE
==================================================

Apply this principle throughout the prototype:

ONE feature
=
ONE primary navigation location.

Do not repeat a feature in multiple menus unless it is a contextual shortcut.

Final mental model:

### Home

Today and upcoming Work Shifts.

### Appointments

Bookings
+
Schedule
+
Booking Policy
per Work Location.

### More

Profile
Patients
Work Locations
Finance
Settings
etc.

### Work Location

Identity / facility information,
not duplicate daily operations.

==================================================
39. CLIENT VIDEO — APPROVED INSPIRATION ONLY
==================================================

From the supplied client weekly-Schedule video,
use ONLY:

- compact weekday visual cards;
- weekly-off selection;
- attractive session blocks;
- session names such as Morning/Evening;
- session time range;
- computed appointment count;
- clear Add Session interaction;
- clear Edit Session Sheet.

DO NOT add from the video:

- VIP;
- VIP allocation;
- arbitrary recurring period end dates;
- N-week recurrence;
- electronic booking toggle per Session;
- booking method duplication per Session;
- unapproved scheduling logic.

==================================================
40. RTL
==================================================

Preserve full native Arabic RTL across all changes.

Especially:

Work Location swipe tabs

Appointments subtabs

Schedule cards

Booking rows

Home Work Shift cards

Finance location tabs

Profile tabs.

Do not regress the recently corrected row structure.

==================================================
41. DO NOT CHANGE FIRST-TIME FLOW
==================================================

New Doctor remains:

Register
→ WhatsApp OTP
→ Specialty
→ Professional Title
→ initial Schedule setup.

Returning Doctor:

Login
→ Home.

==================================================
42. DO NOT CHANGE MONTHLY CALENDAR VISUAL STYLE
==================================================

Final reminder:

The current 30-Day calendar design is approved.

DO NOT redesign it.

Only complete the missing approved interactions/features around it.

==================================================
43. FINAL NAVIGATION QA
==================================================

Before finishing verify that:

- Patients no longer appears in Bottom Navigation.
- Appointments appears in Bottom Navigation.
- Patients is reachable from More.
- Weekly Schedule is NOT duplicated in More.
- Monthly Schedule is NOT duplicated in More.
- Generic Services & Prices is NOT duplicated in More.
- Profile information is unified.
- Work Location does NOT duplicate Schedule/Bookings.
- Appointments switches Work Locations at the top.
- Finance switches Work Locations at the top.
- Hospitals do NOT show Doctor-managed Services tab.
- Online/Private Clinic MAY show Services tab.
- Booking Confirmation Policy is inside Appointments, not generic Settings.

==================================================
44. FINAL APPOINTMENTS QA
==================================================

For every selected Work Location in Appointments verify:

Bookings works.

Weekly Schedule works.

30-Day Calendar works.

Booking Confirmation Policy works.

All are clearly scoped to that selected location.

Do not confuse data between locations.

==================================================
45. FINAL HOME QA
==================================================

Verify Home can show:

Morning shift at برج الأطباء

then:

Afternoon shift at مركز المدينة الطبي

as separate cards.

Each contains the patients belonging to that shift/location.

Doctor can tap:

عرض كل المواعيد

and arrive at Appointments with the correct Work Location already selected.

==================================================
46. DO NOT ADD OTHER FEATURES
==================================================

Do NOT add:

VIP

Waitlist

Queue

Walk-in

Capacity Slot distribution

automatic patient priority

Copy Week

Ramadan logic

appointment buffers

automatic confirmation-window cancellation

new payment functionality.

Keep all other current approved behavior unchanged.