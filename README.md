# SQL-Project-3-Ticket-Administration-Tracker

A fictional internal service desk dataset for tracking requests across IT, Facilities, Human Resources, and Finance. The tables separate departments, staff, tickets, and ticket events so the project can answer day-to-day administration questions.

## Questions explored

- What is in the current ticket queue, and which work is urgent?
- How many active tickets are assigned to each staff member?
- Which tickets are overdue as of the sample reporting date?
- How many tickets does each department handle by status?
- How long do departments take to resolve tickets?
- Which priorities are resolved on time most often?
- How is daily ticket intake changing?
- Are there tickets missing assignment history?

## SQL skills

Primary and foreign keys, `CHECK` constraints, multi-table joins, `LEFT JOIN`, `CASE`, `COALESCE`, `NOT EXISTS`, date and time calculations, aggregates, and window functions (`LAG`).

## Run it

Open `ticket_admin.sql` in a SQLite client and execute the whole file. It recreates its four project tables, inserts fictional sample data, and runs eight reports. The overdue report uses March 24, 2026 as a fixed reporting date so the example results stay consistent.

## Data rules

Tickets in `open`, `in_progress`, and `pending` status count as active workload. `resolved` and `closed` tickets count toward resolution reporting when they have a `resolved_at` value. Staff may be inactive while still appearing in historical tickets; the active-workload report excludes inactive staff.

Authors Note: Ive been working this past weeks on learning all this stuff so now i can post both Projects 2 and 3. Also i'll be releasing AquilonCore Version 0.4 so stay tuned!!!
- SAT
