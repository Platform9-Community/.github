# Contributing to Platform9-Community

Thanks for your interest in contributing. This document covers how to contribute
to any repository in the [Platform9-Community](https://github.com/Platform9-Community)
organization.

## What We're Looking For

Contributions that are useful to practitioners running
[Private Cloud Director](https://platform9.com/private-cloud-director/) -- things
like automation examples, configuration templates, integration patterns, and
operational tooling. If you built something that solved a real problem in your
PCD environment, it probably belongs here.

## How to Contribute

**Platform9 team members** can contribute directly via a branch and pull request
in the relevant repository.

**External contributors** should fork the relevant repository, make changes in
the fork, and open a pull request against the `main` branch.

In both cases, every change goes through a pull request. Direct commits to `main`
are not permitted.

### Step by Step

1. Find the right repository for your contribution, or open an issue if you're
   unsure where it belongs
2. Fork the repo (external) or create a branch (team members)
3. Make your changes
4. Open a pull request with a clear title and description of what you changed and why
5. A maintainer will review and merge it, or follow up with questions

## Pull Request Guidelines

Keep pull requests focused. A PR that adds one well-documented example is easier
to review than one that adds five at once.

Include a clear description. Explain what the contribution does, what problem it
solves, and any environment-specific prerequisites a reviewer should know about.

Add a README if your contribution is a new example directory. Follow the structure
used by existing examples in the repo -- prerequisites, usage, variables, and notes.

Don't commit secrets. No credentials, RC files, `.tfstate` files, `terraform.tfvars`
files, or `clouds.yaml` files. The `.gitignore` in each repo covers the most common
cases, but check `git status` before pushing.

## AI-Assisted Contributions

Contributions that were written or assisted by AI tools are welcome. By submitting
a pull request you are certifying that you have reviewed the contribution, understand
what it does, and take responsibility for its correctness -- regardless of how it
was generated. Do not submit AI-generated content you haven't read and tested.

## Testing

Where possible, validate your contribution before submitting:

- **Terraform**: Run `terraform init` and `terraform plan` successfully against a
  PCD environment. If you don't have access to a PCD environment, note this in the
  PR description and a maintainer will validate it.
- **Ansible**: Run the playbook against a PCD environment and confirm it completes
  without errors.
- Other contributions: describe how you verified the contribution works.

We understand that not everyone has a PCD environment available. Untested
contributions are still welcome -- just be upfront about it in the PR description.

## Code of Conduct

Be respectful and constructive. We're all here to build useful things for the PCD
community. Contributions and conversations that are hostile, dismissive, or
exclusionary will not be tolerated.

## Questions

Open an issue in the relevant repository. If you're not sure which repo applies,
open an issue in this one and we'll point you in the right direction.
