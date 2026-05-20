---
name: bottom-up-tam
description: >
  Build a defensible bottom-up TAM (total addressable market) for a startup pitch
  using the formula ACV × customers in ICP, then show the path to $10M and $100M ARR.
  Use when sizing a market, drafting a TAM slide, sanity-checking whether a business
  is venture-scale, or evaluating someone else's market sizing.
  Triggers: "size this market", "bottom-up TAM", "TAM slide", "is this venture scale",
  "how big is this opportunity", "draft market sizing", "what's the TAM",
  "market sizing", "size the opportunity".
---

# Bottom-Up TAM

> Methodology by **Kabir Dhillon**, originally shared in a Founder University talk (This Week in Startups). Packaged as a Claude Code skill by Ian Pilon.

Build market sizing from the founder's actual pricing and customer count, not from top-down market reports. Credibility is the game, not size.

## The formula

**TAM = ACV (annual contract value) × number of customers in the ICP**

Then always show the path:
- Customers needed to hit **$10M ARR**
- Customers needed to hit **$100M ARR** (the venture-scale benchmark — yields ~$1B valuation at 10x revenue multiple)

## Step 1: Gather inputs

Before drafting anything, ask the user for the inputs below. Do not invent numbers.

1. **Product** — one sentence
2. **ACV** — annual contract value. If pre-revenue, use the assumed future price. If tiered, weighted average. If usage-based, average revenue per customer per year. If marketplace, take rate × average transaction × transactions per year.
3. **ICP** — *specific*, not "anyone 18–80". Include geography, role, company size, vertical.
4. **Customers in ICP** — a defensible count with a derivation path (e.g., "220,000 pediatricians in the US, source: AMA"), not a McKinsey-style black-box number.
5. **Business model** — B2B / B2C / marketplace / tiered / multi-ICP
6. **Go-to-market** — concretely how you reach them (cold call, channel partner, content, paid acquisition)

If any of these are missing or vague, stop and ask. Garbage in, garbage TAM.

## Step 2: Pick the right model

**B2B high-ACV** (e.g., $12K+ ACV)
- Simple ACV × customers
- Highlight: few customers needed → fast to scale
- Example: $12K × 3M ICP = $36B TAM; only 834 customers to $10M ARR

**B2C low-ACV** (e.g., $120/yr)
- Same math, but the path to $100M looks scarier
- Counter by showing % of beachhead needed (e.g., "22% of our 3.7M beachhead = $100M ARR")
- Lead with beachhead, not the full TAM

**Marketplace**
- Estimate transactions, not customers: users × transactions/year × take rate × avg transaction value
- Introduce *both* sides of the marketplace (supply and demand) in the story
- The customer is whoever pays — focus storytelling on them
- Watch for the trap: a small marketplace ($140M TAM) requires 60–70% market capture to reach $100M ARR — almost never credible

**Tiered or usage + subscription**
- Compute a weighted ACV across tiers
- If one revenue stream isn't venture-scale (e.g., usage-based <5% of revenue at scale), visually downweight it so the investor focuses on the durable line

**Multiple ICPs**
- Justify with data: "highest cold-call conversion rates were pediatricians (31%) and family practitioners"
- Don't pick ICPs because they're convenient; pick because evidence points there
- If two roles must agree inside one buyer org, that's *one* ICP (the company) with two decision-makers, not two ICPs

## Step 3: Run the credibility check

Flag any of these before finalizing:

- **Wide ranges**: "everyone 18–80 in the US" — kills credibility
- **Vague segments**: "any B2B SaaS" — ignores that enterprise sales ≠ SMB sales
- **Black-box citations**: "McKinsey says recruiting is $300B" — what's in that $300B, and are you selling all of it?
- **Required market share >10%**: needing 50% capture is unrealistic (Tesla is <10% of US cars)
- **TAM/SAM/SOM stack** with no math — pick one number and derive it
- **Boiling the ocean**: 5+ products/use-cases at once with no execution proof
- **Premature expansion**: "we'll launch in 7 countries year 1" — investors want focus first, expansion as a natural follow-on

**The 20-second test:** could an investor follow the math in 20 seconds and believe each number is derivable? If not, simplify.

## Step 4: Structure the output

Frame as a *journey*, not a destination. Order matters:

1. **ICP + beachhead market** (specific, narrow, defensible)
2. **Go-to-market** (how you actually reach them)
3. **The math, said out loud**: "Our ACV is $X. We have Y potential customers. TAM = $Z."
4. **Path to scale**: "We need N customers for $10M ARR, M customers for $100M ARR."
5. **% of market**: "$100M ARR is only K% of our ICP." (Single-digit is ideal.)
6. **Expansion (optional, cautious wording)**: "After dominating vertical X, the natural next market is Y *because* [shared customer, shared problem, shared distribution]."

Verbalize the math on the slide. Some investors read, some listen — do both.

## Step 5: Stress-test against precedent

Successful companies started narrow and expanded slowly:
- Amazon → books only, for years
- PayPal → eBay power sellers (~20K people, called "terrible customers" at the time)
- Hims & Hers → ~10 years US-only before international
- Duolingo → only recently added math/chess/music after years of language-only

If the founder wants to skip the narrow start, push back: "when it's for everyone, it delights no one."

## Edge cases

**Bottom-up number comes out huge ($60B+):** Fine *if* every input (ACV, customer count, transaction frequency) is independently defensible. Don't shrink the number — pressure-test each assumption until it survives investor scrutiny, then re-multiply.

**Market doesn't exist yet (blue ocean):** Bottom-up is harder because the customer count is speculative. Replace the customer count with a concrete narrative about *why* the market will exist, then make the speculation explicit. Investors will accept speculation if it's labeled honestly.

**Small beachhead can't reach $100M:** Show how you expand — new products to same customers (preferred), or geographic expansion (justify *why* expansion beats upselling). Watch for the focus question: can this founder win the next geography without losing the first?
