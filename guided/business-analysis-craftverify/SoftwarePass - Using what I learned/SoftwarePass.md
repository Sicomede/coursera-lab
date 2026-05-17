# Business overview: SoftwarePass

### Overview

SoftwarePass is a B2B trial-infrastructure platform that lets software vendors embed a "Try in browser" button on their marketing pages, with the actual product running in a streamed, isolated sandbox session. End users evaluate real software without installing anything, and vendors receive high-signal trial telemetry, conversion data, and qualified-lead routing in return. The platform sits between the vendor's marketing site and their own product, replacing static demos, gated downloads, and screen-capture walkthroughs with a live, time-boxed evaluation environment.

### Target consumer profile

**Primary customer (vendor side):**

- B2B and prosumer software companies with download-and-install or complex onboarding flows
- Annual revenue range 2M to 200M USD
- Product-led growth teams, demand-generation marketers, and developer-relations leads inside those companies
- Currently spends real budget on demo infrastructure, trial-conversion tooling, sales-engineer time, and product-led-growth telemetry

**Customer classification:**

- The PLG marketing lead whose current "free trial" requires a 400MB download and a Windows-only installer. Power user. Brings in adjacent vendors at conferences.
- The sales-engineering manager at a mid-market vendor whose team burns hours running one-on-one Zoom demos that should have been self-serve. Buys to recover SE capacity.
- The indie or small-shop software vendor whose ideal customer never makes it past the install step. Buys because the conversion math works at any price point under the lost-trial cost.

**Secondary user (end-user side):**

- Age range 22 to 55
- Software evaluators inside target companies, plus prosumers and developers comparing tools
- Does not pay for SoftwarePass directly, but generates the signal vendors are buying
- Values being able to try before installing, without sales contact, on any device including locked-down work laptops

### Strategic goal and vision

To become the default trial layer for B2B and prosumer software, the way Stripe became the default payment layer. Long-term: when a vendor ships a new product, "wire up SoftwarePass" is a standard line item alongside analytics and billing, and "Try in browser" is the expected affordance on every software marketing page.

### Status of the business

The business is a startup in the prototype validation phase. A single-vertical pilot, likely developer tools or creative software, is being scoped to test whether vendors will pay for trial-session infrastructure on a per-session or subscription basis, and whether the resulting trial-to-paid conversion lift justifies the price. The streaming substrate exists in proven form through Kasm and Cameyo, so technical risk is lower than market-adoption risk.

### Competition

SoftwarePass has no direct competitor positioned around vendor-paid, browser-streamed trial sessions for arbitrary software. Indirect and substrate-adjacent competition is significant and includes:

- Kasm Workspaces and Cameyo, which provide the streaming substrate but sell enterprise app delivery rather than vendor-paid trial infrastructure
- CodeSandbox and StackBlitz, which prove the streamed-trial model works inside the developer-tools vertical but do not generalize
- Guideflow and Navattic, which produce captured interactive demos for sales but run on screen-recordings rather than real software
- Setapp and similar bundle subscriptions, which solve software access but require install and target end users rather than vendors
- In-house demo environments and one-off "trial VMs" that vendors build themselves, which represent the budget SoftwarePass would consolidate
- Product-led growth telemetry tools like Amplitude and Heap, which capture trial behavior but only after the user has already installed

The closest adjacent player is Guideflow, working the demo-sandbox angle but for sales demos on captured screens rather than live software evaluation.

### Business needs

- Streaming and sandbox infrastructure team with experience in low-latency remote rendering and container isolation
- Two or three lighthouse vendor partners in a single vertical, willing to pilot in exchange for case-study rights
- Cloud compute partnerships with committed-use discounts to manage the per-session cost floor
- Conversion analytics and telemetry pipeline that turns session data into the signal vendors will pay for
- Sales motion targeting PLG marketing leads and sales-engineering managers, not procurement
- Legal counsel on software licensing pass-through, end-user data handling, and vendor IP protection inside sandboxes
- Embeddable JavaScript widget and CMS plugins for the major marketing-site platforms

### Trial-session business process steps

1. The software vendor signs up at the SoftwarePass dashboard, selects a plan tier, and uploads or links the software build to be sandboxed.
2. SoftwarePass packages the build into a streamable sandbox image, configures session limits (duration, region, hardware profile), and returns an embed snippet plus a hosted "Try in browser" landing URL.
3. The vendor places the embed snippet on their marketing pages, or links the hosted URL from existing CTAs.
4. An end user clicks "Try in browser" and is dropped into a streamed sandbox session running the real software, with a visible session timer and optional sign-in for saving state.
5. During the session, SoftwarePass captures interaction telemetry: feature usage, time-to-first-action, session depth, drop-off points, and explicit user signals like "save my work" or "request pricing."
6. Tier-dependent path:
   - Starter tier: capped monthly sessions, basic conversion analytics, single sandbox image, SoftwarePass branding visible.
   - Growth tier: higher session caps, full telemetry dashboard, multiple sandbox variants for A/B testing, custom branding, lead-routing webhooks to CRM.
   - Enterprise tier: dedicated capacity and region pinning, SSO and compliance controls, white-label embed, integration with the vendor's PLG stack and BI warehouse.
7. At session end, the user is offered a vendor-defined next step: account creation, pricing page, sales contact, or extended trial through the vendor's own onboarding.
8. The vendor receives session-level and aggregate reporting in their dashboard, including trial-to-paid conversion attribution once the conversion event fires from their side via webhook or postback.
