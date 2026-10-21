# Matchall ChatGPT review preparation

Status: preparation only. No completed target-host case or demo recording is claimed.
The package points to https://matchall.net/amatch/v2 with OAuth and PKCE S256.
Keep the separate legacy awiki.info connection intact. Installing a source ZIP,
connecting a private custom MCP, and verifying the saved submission are different
steps and must be recorded separately.

## Account setup

Use dedicated reviewer accounts that contain only synthetic data. Authenticate
through the host UI; never put passwords, tokens, OTPs or account IDs in public
package files. Account access must remain usable without the owner's private
mailbox or phone. Supply account instructions through the portal's secure reviewer
fields. For the email-code method, follow the current portal's designated reviewer
identity and verify access before submitting. No reviewer account has been provisioned
by this preparation. Do not substitute example.com fixture contacts for a real login.

## Fixtures and cases

Use docs/review-cases.json and its exact matching manifest cases. Choose a fresh
REVIEW run label for each run and replace the example label consistently in every
prompt. Buyer: a used M2 Mac mini, 16 GB RAM, 512 GB SSD, working condition and proof
of purchase, Singapore collection, budget SGD 600. Seller: the compatible item for
SGD 550, same location, with proof of purchase and normal wear. Contacts are the
synthetic strings review-buyer@example.com and review-seller@example.com. Neither
is a receiving mailbox. Keep both records private. No fixtures were created by
this preparation.

1. Complete OAuth, discover tools and call get_profile. Do not create business
   records as part of that initial connectivity check.
2. P1: create and inspect the draft. Only in a separate turn approve confirmation
   and activation. Verify that the same intent is active and is_public is false.
3. P2: read the actual match. Explain unknown fields and product-fit verification;
   do not claim that scores are transaction probabilities.
4. P3: review the exact buyer contact version and explicitly request exchange only
   for the demo seller match. Pending requests must withhold seller contact data.
5. P4 setup: the independent seller uses the Matchall website to review and accept
   that exact request. Then test buyer-side authorized retrieval in ChatGPT. This
   does not claim seller-side respond_contact_exchange was tested inside ChatGPT.
6. P5: pause the intent and inspect the returned lifecycle; do not close, fulfill
   or claim deletion.
7. Run N1 payment, N2 unauthorized contact export and N3 complete-erasure claims.
   Explain the limitations without substitute tool actions or fabricated success.

Record actual arguments/results and each case's Passed/Failed/Blocked/Not run
status in the evidence record. Never expose counterpart data from other matches.
The five positive/three negative cases are authored, not executed evidence.

## Real demo recording

Rehearse the above in the intended ChatGPT development connection first. Record
roughly 2–3 minutes showing connection, the draft and separate approval, actual
matching, pending versus mutually approved contact access, pause and one negative
case. Keep login details and unrelated chats off screen. Recording capability and
host authorization must be available before capturing real evidence; screenshots
or generated slides do not replace a recording. Play back the saved video to check
readability and coverage. The publisher chooses a reviewer-accessible hosting
location. Verify playback without private access, then populate demo_recording_url.
A script or an unhosted local file does not complete this field.

## Final portal steps

Complete publisher identity, support/privacy/terms URLs, country targeting and
commerce declarations before calling the package ready. After an authorized draft
upload, inspect the exact saved version, connect OAuth and run the relevant cases.
Complete required domain verification, security checks and owner attestations.
Submission for review and publication require their corresponding authorization.
