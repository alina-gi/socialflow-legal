# Pre-submission confirmation checklist

The public pages use only the implementation facts currently supported by the SocialFlow TikTok integration audit. Confirm these items before submitting the app for production review.

## Legal and contact details

- [ ] Add a monitored, private contact email or support form to the homepage, Terms, and Privacy Policy. A public GitHub issue is only a temporary contact route; users must not post personal data there.
- [ ] Confirm the operator's legal name, country, and—if counsel recommends it—governing law and business address.
- [ ] Have the Terms and Privacy Policy reviewed for the operator's jurisdiction and intended users. These drafts are not legal advice.
- [ ] Confirm whether the app is single-operator/internal, invite-only, or intended for general public distribution.

## Data practices

- [ ] Identify every AI/model provider used in production and document whether prompts, captions, media, account data, or identifiers leave the device.
- [ ] Confirm whether the app uses telemetry, crash reporting, remote logs, cloud storage, or other service providers.
- [ ] Document the exact retention periods and tested deletion steps for tokens, local media, generated content, logs, and backups.
- [ ] Confirm whether any data is used for model training, analytics, advertising, sale, or cross-context behavioral advertising; update the policy with the truthful answer.
- [ ] Verify the current TikTok scopes and remove any scope not demonstrated and required.

## TikTok review

- [ ] Ensure the working web app domain shown in the review demo matches the Website URL submitted to TikTok, or confirm with TikTok that the selected Desktop flow is reviewed under the applicable rule.
- [ ] Record an end-to-end sandbox demo showing each requested product and scope.
- [ ] Keep captions, hashtags, privacy, interaction, and posting choices editable and under the user's control.
- [ ] Verify the Terms, Privacy, and Web/Desktop URL properties in the TikTok Developer Portal. If URL-prefix verification is used, add TikTok's exact signature file and verify it is publicly reachable.
- [ ] Do not use the GitHub Pages address as an OAuth callback; this static site cannot process OAuth authorization codes.

## Repository separation

- [ ] Confirm this public repository contains no private app source, credentials, `.env` files, access tokens, local vaults, keys, user content, logs, or account screenshots.
