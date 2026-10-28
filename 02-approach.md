# 02. Approach: How I Thought Through the Solution

I structured the work with the CIRCLES method and treated every starting assumption as a hypothesis.

## C: Comprehend the situation

- Reframed "LinkedIn for blue-collar" as a **matching and trust problem**, not a "not enough jobs" problem.
- Asked the competitive question honestly: existing job apps and messaging groups already serve this segment, so "LinkedIn but simpler" is not a reason to exist.
- Chose the wedge from LinkedIn's actual strength, which is professional identity. For tradespeople that translates to **provable skill and career growth**.
- I did not assert any facts about competitors. Their current features need to be checked before any comparison is published.

## I: Identify the customer

- Compared three segments: skilled trades, factory and warehouse, and domestic help.
- Picked **skilled trades (electricians)** because the differentiator (skills proof) works on day one there, and the pilot is geographically contained.
- Built a clearly labelled proto-persona, Murugan. It exists to make design decisions concrete and is meant to be replaced by interview findings.

## R: Report customer needs

Mapped a five-stage journey (Find → Evaluate → Apply → Wait → Start and stay) and attached a hypothesised pain point to each:

| Stage | Hypothesised pain |
|---|---|
| Find | Few nearby, skill-matched options |
| Evaluate | Unclear wage, hours, legitimacy |
| Apply | Text-heavy forms, wrong language |
| Wait | No status or feedback, wasted days |
| Start and stay | Late or unpaid wages, no record of work done |

Two insights drove the design:
1. **"Wait" is underrated.** For someone on daily income, a silent week is a real cost, so status tracking is a core feature, not polish.
2. **Completed work should flow back into the profile.** That is the career-growth loop.

## C: Cut through prioritisation

Separated problems into **table stakes** and **differentiators**:
- Table stakes (necessary but copyable): regional language, voice option, simple navigation.
- Differentiators (the bet): proof of practical skill, vouches, trust signals.

Scored each area qualitatively on impact, confidence, and effort. I deliberately avoided fake numeric scores. Skill proof landed in the *high impact, low confidence* quadrant, which is exactly what to test first.

## L: List solutions

Options considered: voice-first onboarding, Skill Passport, local feed, WhatsApp sharing, employer vouches, wage benchmarks, courses, in-app chat, payments.

**MVP kept:** language and OTP onboarding, Skill Passport with optional proof, local job feed, one-tap apply, status tracking, light trust layer (phone-verified employers, report button, masked contact), and a post-job vouch request.

**Cut:** courses, wage benchmarks, chat, payments. They add scope, trust, and compliance complexity without testing the core bet.

## E: Evaluate trade-offs

| Decision | Chose | Reasoning |
|---|---|---|
| Proof upload | Optional | Required proof would likely reduce profile completion |
| Verification | Light at MVP | Strict verification is high effort and can starve employer supply |
| Voice | Optional add-on | Dialect accuracy is unproven, and not everyone wants to speak to a phone |
| Wage field | Required to post | Wage clarity is central to trust |
| Segment | Skilled trades | Best test of the wedge, even though not the most vulnerable group |

**Key risks:** employer cold start, fake vouches, scams, privacy of photos and phone numbers, bias in ranking, data costs on low-end devices.

## S: Summarise the recommendation

Run a **narrow pilot**: electricians in one city. Ship the Skill Passport, local feed, apply, and status. Validate employer supply and vouch behaviour first, using a manual concierge pilot before building. Expand to adjacent trades only if results meet thresholds set in advance.

**North Star:** verified job starts per week. It's harder to game than applications, though it depends on two-sided confirmation, which is a known measurement weakness.

## Design decisions worth noting

- **Flat navigation** (four tabs): deep menus are a hypothesised barrier.
- **Monochrome wireframes**, with LinkedIn blue (#0A66C2) only on primary actions, so the focus stays on hierarchy.
- **Icon, chip, and voice patterns** instead of assuming low literacy. No formal education does not mean unable to read.
- **"Did you start?" prompt:** it feeds the North Star and also triggers the vouch loop.

## What I'd do next

1. Interview 5 to 10 tradespeople and 5 small employers. Replace the proto-persona.
2. Test the clickable flow with real workers in at least two languages.
3. Run a WhatsApp-based concierge matching pilot.
4. Verify competitor features and add a positioning section.
