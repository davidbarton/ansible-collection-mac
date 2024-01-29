# Ansible collection for macOS setup automation

[![CI](https://github.com/davidbarton/ansible-collection-mac/actions/workflows/ci.yml/badge.svg)](https://github.com/davidbarton/ansible-collection-mac/actions/workflows/ci.yml)

## Release + Publish steps
1. [localhost] Bump version in galaxy.yml, create PR & merge it
2. [localhost] Create git tag (eg 1.0.0) and push
3. [CI:lint] Run lint
4. [CI:test] Run full tests
5. [CI:release:pre-release] Verify Ansible Galaxy token is present
6. [CI:release:pre-release] Verify version in galaxy.yml with tag version
7. [CI:release:build] Build artifact
8. [CI:release:release] Create Github release with auto generated release notes and attach artifact
9. [CI:release:publish] Publish to Ansible Galaxy
