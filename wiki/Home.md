# Welcome to the cruft-spindle-project wiki!

# Notes

This cruft template is to be used for all [Twine](https://twinery.org) Games built using [Spindle](https://github.com/brisberg/spindle) for deployment on `twine.brisberg.dev`.

It's only dependency is `@brisberg/spindle`.

Deployments will trigger an 'update and re-deploy' on `brisberg/twine.brisberg.dev` with the latest version. It does this though a `repository_dispatch` event. Both repositories need to be consistent with how they interact with this event.

Repository Dispatch events cannot be triggered using the default `secrets.GITHUB_TOKEN` so a special `PAT` is required. I have added one to my account, but it must be added as a secret to each repo based on this template to work.
