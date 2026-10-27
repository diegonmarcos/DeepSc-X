# DeepSc-X

DeepScX - member of the [DeepSc](https://github.com/diegonmarcos/DeepSc) hub. No content yet: this repo is a README plus the deployer wiring skeleton (ticket #1224).

Candidate for the pending front-labtools split (#1218), NOT moved now: front-labtools c-Stk_DsX/sailytics (Deep-ScX / saylitics, URL /sailytics/).

## Wiring

- `build.json` (empty build list), `build.sh` and `ship.yml` are symlinks/files that resolve through `1_cicd` and `.github` into the `0_deployer` submodule (diegonmarcos.github.io, shallow, `ignore = all`), as in every front repo (#1192/#1196).
- The deployer clones this repo and overlays it at `a_Companies/deepsc-x`; the project is skipped until `dist/` exists. Its published URL will be `https://diegonmarcos.github.io/deepsc-x/`.
