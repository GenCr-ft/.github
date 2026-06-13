# GenCr@ft Studio

GenCr@ft is building **Aethel**, a multiplayer voxel RPG creative platform.
The organization is split across multiple repositories, so newcomers should not
start by guessing which repo matters.

## New Here?

Start with the public onboarding hub:

**https://gencr-ft.github.io**

It explains the five bounded workspaces and gives the quickstart commands for
Linux, macOS, WSL, and Windows.

## Fast Path

If you already know your workspace, use the onboarding scripts directly:

```bash
mkdir -p ~/gft && cd ~/gft
curl -L https://raw.githubusercontent.com/GenCr-ft/gcd-onboarding-scripts/main/gft-onboarding.sh -o gft-onboarding.sh
curl -L https://raw.githubusercontent.com/GenCr-ft/gcd-onboarding-scripts/main/gft-onboarding.sh.sha256 -o gft-onboarding.sh.sha256
sha256sum --check gft-onboarding.sh.sha256 && bash gft-onboarding.sh --quickstart --workspace aethel
```

Replace `aethel` with `evai-platform`, `agent-factory`, `workspace-ops`, or
`studio-gencraft`.

## Primary Entry Points

- [gcd-onboarding-scripts](https://github.com/GenCr-ft/gcd-onboarding-scripts) - local developer setup.
- [gcp-aethel-server](https://github.com/GenCr-ft/gcp-aethel-server) - authoritative game server.
- [gcp-aethel-client](https://github.com/GenCr-ft/gcp-aethel-client) - Godot client.
- [gcs-plt-tools](https://github.com/GenCr-ft/gcs-plt-tools) - EvolvAI DevSphere platform tooling.
- [gcs-project-management](https://github.com/GenCr-ft/gcs-project-management) - active planning and tracker state.

After cloning a repo, read its `AGENTS.md` first.
