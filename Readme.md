# Monofolio Ops

This is the second part of the Monofolio Project, whith the purpose of having a better workflow.

## Goal

- [ ] Correctly setup the project with separated Code and Infrastructure repositories
- [ ] Create a CI/CD pipeline for the Code repository that will build the application and on success, trigger the Infrastructure repository to update the infrastructure
- [ ] Handle Three Environments:
  - [NOT MVP] Development (with a subdomain {Branch name}.dev.\*)
  - [ ] PreProd (with a subdomain beta.maxleriche.net)
  - [ ] Production (with a subdomain maxleriche.net)

## Trigger for the Code Repository

The build should be triggered by a push to a branch, and then conditional to the file changed (Front/Backend).

The build should be tagged depending on the branch name or if it's a tag.

In case of a tag, the build should be tagged with the tag name and not conditional to the file changed.