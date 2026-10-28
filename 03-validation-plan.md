# 03. Validation Plan and Success Metrics

Nothing in this project is validated yet. This plan shows how each hypothesis would be tested. Set decision thresholds **before** running each test, to avoid explaining results after the fact.

## Hypothesis → test

| Hypothesis | Method | What would support it | What would refute it |
|---|---|---|---|
| H1 Language is a barrier | Moderated usability test of the flow in 2 to 3 languages | Participants finish onboarding faster or with fewer errors in their own language | No difference by language |
| H2 Complex UI causes drop-off | Task test on the clickable prototype | Participants stall on text-heavy steps | They complete tasks without help |
| H3 Workers can't prove skill | Interviews on how they get hired today | Hiring runs on trust and referrals, with no shareable proof | Existing proof (certificates, portfolios) already works |
| H4 Few relevant local jobs | Concierge pilot: manually match jobs through WhatsApp | Workers report irrelevant or distant options today | Workers already find enough relevant work |
| H5 Wages are unclear | Review sample job posts with workers | Wage or hours missing from common posts | Wages are generally stated |
| H6 Employers will post clear wages | Employer interviews and a post-flow test | They complete posting with wage and hours | They refuse or skip those fields |
| H7 Employers will confirm and vouch | Send a vouch link to employers after a real job | A meaningful share tap it | Links are ignored |

## Phases

1. **Discovery:** worker and employer interviews. Replace the proto-persona.
2. **Prototype testing:** usability tests on the clickable flow.
3. **Concierge pilot:** manual matching, no new software, to test supply and demand cheaply.
4. **Small build and pilot:** one city, one trade, an MVP release.

## Interview starters

**Workers**
- Walk me through the last time you found work. What happened first?
- How did you decide whether a job was genuine?
- What do you do when an employer doesn't pay on time?
- How do you show someone you're good at your work?
- Which apps do you use every day, and what do you use them for?

**Small employers**
- How do you find and trust new workers today?
- What would make you share the wage and hours up front?
- Would you confirm that someone worked for you? What would stop you?

## Success metrics

**North Star:** verified job starts per week. Both worker and employer confirm.

| Area | Metric |
|---|---|
| Profile completion | % of new users with at least one skill and one proof item |
| Relevant job discovery | % of sessions where the user views or saves a skill- and distance-matched job |
| Application conversion | Job view → apply rate |
| Employer response | % of applications answered within a set window |
| Job legitimacy | % of posts verified; scam-report rate |

**Guardrails:** report rate, data used per session, crash rate on low-end devices.

**Measurement caveat:** start confirmation depends on both parties responding. Plan a worker check-in at day 7 and day 30, and treat unconfirmed starts as unknown, not as failures.

## Key risks and mitigations

| Risk | Mitigation |
|---|---|
| Employer cold start | Concierge pilot; start with one trade and city |
| Fake vouches | Phone-verified vouchers; weight by employer reputation later |
| Scams and placement fees | Report button, verified badge, wage required on every post |
| Privacy of photos and phone numbers | Masked contact, optional proof, clear consent |
| Low-end devices and data costs | Lite mode, compressed media |
| Voice accuracy across dialects | Keep voice optional; test before relying on it |
