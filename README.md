# 永田｜日本語会話 / 日语聊天练习

Bilingual public lesson information and booking calendar, hosted on GitHub Pages.

## Updating confirmed reservations

The canonical schedule is the JSON inside `index.html`, in `<script id="schedule-data" type="application/json">`.

- Read the current repository version before editing. Preserve every existing confirmed booking unless the owner requests a change or cancellation.
- Owner's chat instructions without a timezone use Asia/Tokyo (UTC+9). Explicit China time uses Asia/Shanghai (UTC+8). Ask if the year or intended date is ambiguous. Do not infer confirmation from tentative conversation history.
- Each booking uses a stable `id`, and ISO 8601 `start` and `end` values with explicit timezone offsets. End must be after start. Detect overlapping bookings and resolve with the owner rather than silently overwriting.
- Publish times only: no student names, contact details, payment information or private notes in this public repository.
- `updatedAt` is the actual time of a calendar edit with an offset; do not set it to page-load time. Preserve it for unrelated design edits. The page displays this timestamp in both timezones.
- Empty days are inquiries, not confirmed availability. Current bookings are intentionally empty until the owner supplies confirmed reservations.
- After a requested chat update, commit the modified file, verify deployment and report the booking times in both timezones plus the calendar update timestamp. There is no background chat listener or automatic reservation intake.

## Content

Monthly plans: 4 × 60 minutes / 138 CNY; 8 × 60 minutes / 272 CNY; 12 × 60 minutes / 396 CNY. Trial: 30 minutes / 10 CNY. Single session: 60 minutes / 35 CNY. No external fonts, scripts, APIs or image services are required.

Detailed cancellation deadlines, refund conditions and other unverified terms must not be invented; the public page directs learners to confirm those before booking.
