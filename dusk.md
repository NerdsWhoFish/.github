---
dusk: v1alpha1
namespace: stout
kind: repository
name: nerdswhofish-github
title: NerdsWhoFish GitHub organization profile
attributes:
  github_repository: NerdsWhoFish/.github
  role: organization-profile-and-shared-workflows
  visibility: public
---

<!-- markdownlint-disable-file MD013 -->

The special GitHub repository for the NerdsWhoFish organization.
GitHub renders `profile/README.md` on the organization's public profile, while `.github/workflows/` contains reusable workflows shared by the Dusk plugin repositories.

The profile is maintained by hand. Its logo is a copy of the approved dark wordmark from the private `NerdsWhoFish/NWF-Branding` source-of-truth repository, because GitHub cannot render an asset fetched from a private repository for anonymous visitors.

## Gotchas

- Keep the root `README.md` focused on repository maintainers. Only `profile/README.md` appears on the organization profile.
- Sync `profile/assets/nwf-logo-dark.svg` when the approved wordmark changes in `NerdsWhoFish/NWF-Branding`.
- Do not replace the local logo with a private raw GitHub URL. It will disappear for signed-out visitors.
