# Contributor agreement rollout

`CLA.md` is the proposed version 1.0 agreement. GitHub uses `CONTRIBUTING.md` from
this repository's default branch for repositories in this organization that do
not define their own contribution file. Changes on a pull request branch do not
publish or update that default until merged. GitHub applies the default
[regardless of the destination repository's visibility](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file#about-default-community-health-files).
Existing repository-specific contribution files must link to the shared agreement.

The signing service is hosted at https://app.typewhisper.com/cla. A single
acceptance is tied to the signer's stable GitHub account ID and the exact
agreement version. The `TypeWhisper CLA` GitHub App check verifies the PR author,
commit authors, and coauthors. Contributor names are not evidence of acceptance.

## Activation checklist

- Review the contract, sublicensing scope, employer authorization, privacy
  notice, and treatment of earlier work before opening the agreement for signing.
- Confirm that the portal displays the exact reviewed version and content hash.
- Install the GitHub App on the participating repositories. Exclude upstream
  forks and archived projects. Review newly created repositories before accepting
  contributions.
- Verify an unsigned contributor fails the check, explicit acceptance makes it
  pass, and an additional unsigned coauthor makes it fail again.
- Require the current agreement's `TypeWhisper CLA` check, including its version
  and content hash in the check name, from the expected GitHub App on default
  branches. Prepare the new required context before activating a replacement
  agreement, then recheck all open PRs. Older successful checks must not satisfy
  the new requirement. Preserve existing required checks and branch protections.
- Where the GitHub plan cannot enforce checks, maintain a manual merge gate and
  record that limitation. Do not change repository visibility to enable a rule.
- Replace the preparation notice in the contribution guides only once the
  signing page and checks are live.

## Review responsibilities

Passing the check is evidence of the configured contributor agreement policy,
not a complete copyright audit. Review third-party code, dependencies, licensing
notices, and employer rights. A contributor can grant only rights they own or are
authorized to license.

The project owner and narrowly identified GitHub automation accounts may be
exempt from signing. An exemption is not a signature and grants no rights to
third-party code. Do not exempt all organization members, usernames matching a
wildcard, or an unknown contributor to make a check pass.

If an author cannot be associated with a GitHub account, ask them to associate
their commit email with that account and request a recheck. Corporate grants need
an authorized representative and a documented scope; an employee's individual
signature alone does not establish their employer's authorization.

## Earlier contributions

Inventory already merged PRs, direct commits, coauthors, and code imported from
other distributions. Record the applicable license and any separately documented
grant. New acceptance must not be recorded as retroactive consent by default.

For each earlier contribution needing additional rights, obtain an explicit
grant identifying the contribution and rights holder, or assess whether it must
be excluded or replaced in a distribution needing those rights. Keep private
repository inventories and personal contact details out of this public repository.

Bug reports and ordinary discussion do not require signing. Upstream forks retain
their upstream contribution rules.
