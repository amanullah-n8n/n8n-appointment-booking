# n8n-appointment-booking
"n8n workflow for automated appointment booking with Google Calendar availability check"
# Appointment Booking Automation (n8n)

This workflow automates appointment booking by:
1. Checking Google Calendar availability for a requested time slot
2. If the slot is free, automatically creating a calendar event
3. If the slot is busy, returning a "not available" message

## Tools Used
- n8n (workflow automation)
- Google Calendar API
- Date/Time expressions (Luxon library)

## How It Works
1. Takes customer name, appointment date, and time as input
2. Checks calendar availability using Google Calendar's "Get Many Events"
3. IF condition determines if the slot is free or busy
4. Creates event automatically if available, prevents double-booking if not
