# Design QA — GitHub organization profile

- Source visual truth: `/Users/idonghyeon/.codex/generated_images/01a09f57-8d4c-7d90-8ac2-2359baff27e4/exec-ab2ec312-243c-47cb-8aad-3a3ee77b2571.png`
- Desktop implementation: `design/implementation-profile-software.png`
- Mobile implementation: `design/implementation-profile-mobile-software.png`
- Side-by-side evidence: `design/qa-comparison-v2.png`
- Desktop viewport: 1440 × 1100 CSS px, device scale factor 1
- Mobile viewport: 390 × 844 CSS px, device scale factor 1
- Source pixels: 887 × 1774
- Desktop implementation pixels: 1440 × 1882
- Mobile implementation pixels: 390 × 3124
- State: public organization Overview README, light GitHub surface

## Full-view comparison

The selected direction and implementation were viewed together in `design/qa-comparison-v2.png`. The implementation retains the selected direction's navy photographic hero, Korean-first value proposition, four delivery capabilities, applicable-work section, six-stage delivery process with outputs, and dark project-inquiry close. The GitHub-ready version deliberately uses fewer photographs because institution-like imagery could imply unverified clients or work history.

## Required fidelity surfaces

- Fonts and typography: Korean hierarchy, bold display weights, restrained English labels, and readable line height match the selected direction. Desktop explanatory copy was enlarged after the first pass. Mobile-specific 360px assets preserve approximately 12–14px rendered body text instead of shrinking the desktop graphics.
- Spacing and layout rhythm: Major sections follow the source order and alternate white, light-blue, and navy surfaces. Desktop uses four- and six-column structures; mobile uses two-column structures to prevent horizontal overflow.
- Colors and visual tokens: Deep navy `#061b3e`, blue `#1681ef`, white, muted blue-gray text, and light-blue section surfaces are consistent across all assets.
- Image quality and asset fidelity: The supplied H mark is reused. The hero uses a generated enterprise software topology showing application, service, integration, and data layers without depicting a client system. No institution signage, customer logo, performance claim, badge, or placeholder image is present. Desktop assets are 1600px wide; mobile variants are rendered at their 360px target width.
- Copy and content: Service taxonomy, AX positioning, domain, and email match the approved company copy. Applicable examples explicitly say they are not completed-project results.

## Focused-region comparison

- Hero: the implementation preserves the selected composition and value statement while replacing the architectural/coastal visual with a neutral software topology of application, service, integration, and data layers.
- Applicable work: the implementation keeps four scannable categories and adds an explicit non-performance disclaimer.
- Delivery process: the implementation retains six steps and adds concrete outputs. The mobile version reorganizes the same content into a 2 × 3 grid.
- Contact: website and email are visually separated and remain functional links in the README.

## Comparison history

### Pass 1 — blocked

- P2: desktop capability descriptions and process outputs became too small at GitHub's approximately 900px content width.
- P2: desktop 1600px graphics were not readable when scaled into a 390px mobile viewport.

### Fixes applied

- Increased desktop capability, applicable-work, process, and output typography and section heights.
- Added dedicated 360px mobile variants for the hero, capabilities, applicable work, process, and contact sections.
- Added responsive `<picture>` sources at a 600px breakpoint.

### Pass 2 — passed

- Desktop and mobile screenshots show no clipping, horizontal overflow, missing imagery, or broken content hierarchy.
- Website, project-inquiry, hero, and contact links are present in the browser accessibility tree.
- Browser console and page-error checks returned no errors.

### Hero refinement — passed

- Replaced the architectural/coastal hero with an enterprise software topology; the right-hand visual now reads as connected applications, services, APIs, servers, and databases.
- Desktop and dedicated mobile captures preserve the copy hierarchy without clipping, overflow, or loss of contrast.
- Browser console and page-error checks returned no errors after the replacement.

## Residual P3 polish

- The final GitHub-rendered result should be checked after pushing because GitHub may sanitize or reinterpret the `<picture>` media attributes.

final result: passed
