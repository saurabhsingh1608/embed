
# ThoughtSpot CI

Manage your ThoughtSpot objects with the [__Verion Control APIs__](https://developers.thoughtspot.com/docs/rest-apiv2-reference#_version_control) and [__Github Actions__](https://github.com/features/actions).

## Quickstart

  1. __[Fork this repo](https://github.com/thoughtspot/tsci/fork)__.
  2. Create a new branch, one for each ThoughtSpot Org managing content.
  3. [__Configure your GitHub Secrets__](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions#creating-secrets-for-a-repository) to manage authenticatation to ThoughtSpot.
  4. Customize the [__workflow files__](.github/workflows/) to your needs.

## Which Secrets do I have to manage?

__ThoughtSpot__ [requires an authenticated session](https://developers.thoughtspot.com/docs/api-authv2) in order to use the APIs. Each of the workflows will ask for 3 secrets.

  - `THOUGHTSPOT_URL` - your ThoughtSpot URL (eg. https://company.thoughtspot.cloud)
  - `THOUGHTSPOT_USERNAME` - an Administrator-level username
  - `THOUGHTSPOT_SECRET_KEY` - your cluster-level ThoughtSpot [__secret key__](https://developers.thoughtspot.com/docs/trusted-auth-secret-key#_secret_key_overview)

## How to Use / Guides

  1. [How do I fetch changes made in ThoughtSpot?](info/commit.md)
  2. [How do I open a Pull Request?](info/validate.md)
  3. [How do I deploy changes to a new ThoughtSpot environment?](info/deploy.md)
