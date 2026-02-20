# Problem Statement V1: Recording/Production Studio Booking Systems

**Date Created:** January 20, 2026  
**Target Segment:** Recording & Production Studios, Tulsa/NW Arkansas Region  
**Status:** Hypothesis - Testing with first 5 clients

---

## Problem Statement

Independent recording and production studios in the Tulsa/NW Arkansas region struggle to coordinate bookings because available software can't model the complex constraints of time, room, equipment, and staff expertise. Studio owners like Sarah spend hours reconciling double-booked calendars, manually tracking which gear and people are where, and fixing costly scheduling errors—often after losing clients or revenue. Mainstream tools treat each resource as independent, while real studios need a system that sees bookings as a constraint graph: the right room, the right setup, the right engineer, all at the right time.

---

## Observable Behavior (Sarah's Story)

Sarah owns a recording studio with 3 rooms:
- **Studio A:** Full band setup with live room
- **Studio B:** Podcast/voiceover booth  
- **Studio C:** Mixing and mastering suite

**Every Sunday night**, she spends 2-3 hours reconciling her booking system (which only knows about time slots) against a color-coded Google Sheet that tracks which equipment is in which room and which engineer is qualified for which setup. 

**Tuesday afternoon**, a client books "Studio A" online but needs podcast recording—Sarah texts them: *"Hey, Studio B is better for podcasts, can we switch you?"* Client gets confused, cancels. She loses **$400** and spends another hour updating the sheet to block that slot differently.

---

## Key Insights

1. **Studios routinely lose time and money despite paying for "automated" booking/scheduling tools**
   - Current tools: Calendly, Acuity, Square Appointments, basic WordPress plugins
   - Price paid: $50-$200/month for tools that don't solve the core problem

2. **The pain peaks after off-the-shelf solutions and basic custom builds have failed**
   - Trigger moment: After spending $3K-$8K on a website/booking system that created MORE manual work
   - Emotional state: Embarrassment, frustration, feeling "not tech-savvy" when the tools are actually broken

3. **Constraint-aware bookings represent a repeatable and urgent problem across the local creative community**
   - Every studio has the same structural challenge: multi-dimensional resource constraints
   - Studios network and refer to each other—word-of-mouth potential is high

4. **The solution requires modeling real-world dependencies, not just digital forms**
   - Root cause: Booking tools model `Time x Service = Booking`
   - Studio reality: `(Time x Room x Equipment x Staff Qualifications x Client Need) = Valid Booking`

5. **Typical impact: 10-15 hours/week in manual coordination, $400-$1,200/month in lost revenue from booking errors or client confusion**

---

## Technical Root Cause

Off-the-shelf booking platforms treat resources as **independent variables** when studios need **constraint graphs**.

**What fails:**
- Client books "Studio A" → System confirms → Owner discovers equipment conflict later
- No validation of: Is the right room available? Is the equipment in that room? Is a qualified engineer scheduled?

**What's needed:**
A system that enforces multi-dimensional constraints at booking time:
```
Valid Booking = f(time, room, equipment_state, staff_expertise, client_requirements)
```

Where the system automatically:
- Routes podcast clients to podcast-optimized rooms
- Checks equipment availability across all rooms in real-time
- Matches engineer qualifications to client needs
- Prevents double-booking at the equipment level (not just time slots)

---

## Target Customer Profile

**Industry:** Recording studios, podcast studios, video production spaces, rehearsal facilities  
**Location:** Tulsa/NW Arkansas region (2-3 hour drive radius)  
**Revenue:** $150K-$500K annually  
**Size:** 1-3 staff members, 2-5 physical spaces  
**Current Tools:** Calendly/Acuity + Google Sheets/Excel + text messages  
**Pain Level:** Acute (losing revenue, spending 10+ hours/week on manual coordination)  
**Budget:** Can't afford $20K-$50K enterprise solutions, already spent $3K-$8K on failed attempts

**Founder-Market Fit:**
BTS founder is a music producer with hands-on studio operations experience. The booking/resource management system being built for clients is the same system needed for BTS's own studio capabilities (development, recording, filming). This ensures:
- Real-world validation through daily operational use
- Deep domain expertise that competitors (generic dev shops, off-the-shelf SaaS) cannot replicate
- Instant credibility with studio owner prospects—speaking as a peer, not an outsider
- Continuous product evolution based on lived experience, not theoretical requirements
- Ability to dogfood every feature before client deployment  

---

## Discovery Questions (Client Calls)

1. What's the one workflow that makes or breaks your week?
2. Where do your current tools/workarounds force you to "duct tape" things together?
3. Have you ever paid (or seriously considered paying) for a custom solution? What stopped you?
4. When was the last time this problem actually cost you time, money, or reputation?
5. Who else on your team—or in your local network—is dealing with the same thing?
6. If you could wave a magic wand, what would just "work"—no tech skills needed?
7. How many hours per week do you spend manually coordinating bookings/equipment/staff?
8. What's the typical cost when a booking error or scheduling conflict happens?

---

## Pattern Recognition Criteria

After 3-5 client projects, validate whether this is a true pattern:

✅ **Pattern Confirmed If:**
- 3+ studios describe the same broken process unprompted, in their own words
- They converge on the same "must-have" features with budget attached
- 60-80% of the technical solution is identical across clients (only surface tweaks needed)
- Prospects are finding BTS because of word-of-mouth about solving this specific problem
- A 70% core solution could serve 80% of clients with minor customization

❌ **Pattern Disproven If:**
- Each studio's core needs diverge significantly
- No willingness to pay for a solution ($3K+ custom or $200-500/month SaaS)
- The "spreadsheet workaround" is acceptable to most studios
- Other pain points emerge as more urgent than booking/resource management

---

## Next Steps (48-Hour Execution Plan)

1. **Network Activation (Today):**
   - Reach out to Gradient contacts and OKSBDC referrals
   - Ask: "Who do you know running a recording/production studio that's frustrated with their booking system?"
   - Offer: Free 30-minute workflow audit

2. **First Discovery Call (By Friday):**
   - Use discovery questions above
   - Document: client type, pain moment, current workaround, dollars at stake, tools rejected
   - Validate: Does Sarah's story resonate? Do they nod and say "yes, that's exactly me"?

3. **Pattern Documentation:**
   - After each client call/project, update pattern tracking spreadsheet
   - Review pattern map after clients #3, #5, and #8
   - Decision point at client #5: Double down on studios or pivot to adjacent segment?

---

## Business Model Hypothesis

**Revenue Streams:**
1. **Custom Development:** $3K-$8K per studio for tailored booking/resource management system
2. **Productized SaaS (Future):** $200-$500/month after pattern validation and 70% core build

**Lean Operations:**
- Launch with AI-assisted development to minimize costs
- Scale to human developers as revenue justifies
- Prioritize Atlas School alumni and local Tulsa tech talent

**Break-Even Target:** 8 months (based on 5-10 custom client projects + early SaaS adopters)

---

## Success Metrics (90-Day Sprint)

- **Client Conversations:** 10+ studio discovery calls
- **Paid Projects:** 3-5 custom builds ($3K-$8K each)
- **Pattern Validation:** Clear evidence of repeatable 60-80% core solution
- **Revenue:** $15K-$30K (enough to extend runway and hire first dev if needed)
- **Referrals:** 2+ warm introductions from satisfied early clients

---

**Last Updated:** January 20, 2026  
**Owner:** Demond Balentine Sr., Founder & Technical Lead, BTS  
**Next Review:** After Client #3 (estimated late January/early February 2026)
