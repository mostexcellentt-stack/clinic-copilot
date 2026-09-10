# clinic-copilot - Two-Day Follow-Up
Outbound CALL-E skill for clinics.
PROBLEM: Clinics lose track of patients after visits.
SOLUTION: CALL-E calls patient 2 days later, checks recovery, books follow-up.
HOW IT WORKS:
- Input: patient_name, visit_date
- CALL-E asks: better / same / worse?
- If worse or missed medication -> needs_nurse_callback = true
- Offers: tomorrow 10am or 2pm
- Output JSON: patient_name, feeling, needs_nurse_callback, follow_up_booked
TESTED & PASSED: Daniel felt worse, missed meds -> flagged for nurse, booked tomorrow 2pm.
SAFETY: No medical advice.