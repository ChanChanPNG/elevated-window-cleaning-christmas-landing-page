# Elevated Christmas Lights — Vercel landing page

This static site uses **real Elevated project photos**, the provided business logo and owner photo, and the **supplied GHL form embed**. The form iframe loads from LeadConnector; submissions go through that embedded form, not through custom site JavaScript.

## Deploy
Upload the contents of this directory to a GitHub repository, then import into Vercel as a static site with no build command. Set a custom domain if desired.

## Connected form
Form ID: `0vOx5JC7BBK2NHhsucTt`. The official resizing script is included. The initial iframe height is 1468px. Test on mobile and desktop; the GHL editor governs the actual inner form appearance, validation and consent.

## Before running paid ads
- Submit a test form and confirm the contact is created in the correct Elevated GHL subaccount.
- Configure its GHL form success redirect and/or success message (e.g. an approved thank-you page), workflows, owner notifications, pipeline, and consent.
- Connect Meta Pixel and properly configured server Lead events; these are **not** installed in this bundle.
- Test UTM/fbclid capture on the externally embedded form; do not assume iframe attribution works.
- Confirm service wording, privacy terms, and holiday scheduling.
- Confirm whether the client approves displaying the provided photos and owner portrait.
- Confirm Jobber handoff and revenue reconciliation.


## October 24 revision
- Heading accent text uses the **same font and upright styling**, with gold color only.
- Desktop navigation remains visible during scrolling; mobile has a fixed cranberry estimate CTA.
- GHL iframe now uses eager loading instead of lazy loading, and the official resize script loads deferred.
- For intermittent empty embeds, also test in an incognito browser with extensions disabled, check cookie/consent blockers and third-party iframe requests, and inspect GHL form publishing settings. A successful live submission is still required.
- The empty fourth change item was not implemented because no details were supplied.

## October 24 revision — footer and phone links
- Removed both publicly displayed phone numbers/phone links from the landing page (estimate section and footer). The GHL form’s required customer phone field is unchanged.
- Added the cropped compass mark from the user-supplied Wayfinder Creative logo next to the “Designed and hosted by Wayfinder Creative” footer credit, linking to wayfindercreative.net.


## October 28, 2026 — Legal & Compliance update
Added four dedicated legal pages: `privacy-policy/`, `terms-of-service/`, `sms-policy/`, `anti-spam/`. The footer now links to all four on the landing page and on each legal page. Added a concise privacy/SMS notice adjacent to the estimate form; this does **not** replace actual GHL checkbox disclosures. Policies are business-specific drafts requiring business verification and legal review.

**Before launching any marketing:**
- Confirm the precise registered LLC name and state, policy accuracy, and data-processing/retention practices.
- Inspect GHL embedded form ID `0vOx5JC7BBK2NHhsucTt` for separate, unchecked and appropriately worded SMS/marketing consent where legally required; capture timestamp, disclosure version, source, and consent status. Test STOP and HELP, internal suppressions, and A2P registration. No changes to the third-party iframe's internal consent fields were made.
- Set a valid physical postal address in outgoing commercial marketing emails, and test unsubscribe handling; no mailing address was supplied for this project.
- The source ZIP README explicitly states that Meta Pixel is **not installed** in this bundle. If Pixel or other nonessential tracking is installed later, update policies and implement any required opt-in/cookie controls, as appropriate.
- Confirm Jobber/Stripe/Meta actually receive or process information in the live production workflows; tool descriptions in policy are qualified accordingly.
- Verify legal page URLs and GHL form at the real deployed domain. For Vercel static hosting, folder `index.html` pages generally resolve to clean paths, but confirm deployment and any redirects.
