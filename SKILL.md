# Clinic Copilot - Two-Day Follow-Up

Outbound CALL-E skill for clinics - Most Practical Category

Problem: Clinics lose track after visits
Solution: CALL-E calls 2 days later

Flow:
1. Greet by name + visit date (e.g. Sept 8th)
2. Ask better/same/worse?
3. If better -> remind finish meds, no callback
4. If worse/missed meds -> needs_nurse_callback=true, offer tomorrow 10am or 2pm
5. Return JSON: patient_name, feeling, needs_nurse_callback, follow_up_booked

Tested: Daniel - feeling worse, missed meds -> callback=true, booked tomorrow 2pm - PASSED

Safety: No medical advice. Emergency -> tell patient to call emergency services.

Dashboard: dashboard.heycall-e.com - Goal published, simulation passed. Nigeria number not supported for real call, so simulation used - valid per hackathon rules.