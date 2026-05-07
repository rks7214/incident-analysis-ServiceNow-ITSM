
 Step 1: User Setup
- Created sample users
- Assigned roles:
  - itil
  - admin
  - itil_admin

 Step 2: Group Setup
- Created a group
- Added users to the group

 Step 3: Flow Designer Configuration

 Trigger
- When: Incident is created

Lookup Records Action
Conditions:
- Configuration item is NOT EMPTY
- State is NOT Closed
- Opened in last 7 days

Condition Logic
- Count incidents
- If incident count ≥ 3 → trigger email

 Action
- Send email to assigned group

 Step 4: Testing
- Created multiple incidents with same Configuration Item
- Verified:
  - Flow execution
  - Email trigger
  - Logs in inbound email
