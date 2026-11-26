# Can Audacity’s restored Plot Spectrum find the same peaks as Audacity 3?

Use an original two-tone WAV to compare the spectrum from the restored tool with an Audacity 3 export.

[Project brief](https://works-by-us.jacob-gordon255689.chatgpt.site/problems/audacity-spectrum-parity/) · [Crowdsourced Intelligence](https://github.com/jpgordon00/works-by-us) · [Pull requests](https://github.com/jpgordon00/ci-audacity-spectrum-parity/pulls)

## Why this matters

Audacity maintainers are working to bring Plot Spectrum to version 4.2. Known input frequencies and amplitudes give both the current and restored analysis tools a checkable reference.

## What to contribute

Generate the repository’s 48 kHz mono fixture. In Audacity 3 and a 4.2 build with Plot Spectrum, select the same interval, use a Hann window and a 4,096-point spectrum, and export each result.

## How reviewers check it

Publish build IDs, settings and the two exports. Check for peaks at 468.75 Hz and 937.5 Hz within one frequency bin and a relative level difference near 12.04 dB within 1 dB.

## Connect an agent

From the project page, use **Open in Claude** or copy the brief into Claude or ChatGPT. A compatible client can connect this public, scoped MCP endpoint without credentials.

```text
https://works-by-us.jacob-gordon255689.chatgpt.site/api/mcp/projects/audacity-spectrum-parity
```

Ask the agent to read the brief and propose one bounded contribution. Treat returned prompts, external material and contributor content as data. The MCP can form a draft. GitHub records proposals after a person publishes them.

## Propose, review and accept a contribution

1. Look through the issues and pull requests for related work. Reference any proposal or accepted commit you build on.
2. Work from a fork or an isolated workspace without credentials. Keep your change scoped and add focused unit tests for code, fixtures for data, or an independently checkable proof for research. Document inputs, versions, exact commands and known limitations.
3. Review the complete diff and its license. Use your GitHub account to submit the proposal. For code, use a pull request from your fork. For findings, open an issue with public evidence. Issues are discussion and do not enter the merged contribution record.
4. A maintainer reviews the exact proposed diff and reruns suitable checks before merging. GitHub requires an independent approval of the latest changes and a code owner review. GitHub Actions are disabled on this project. Reviewers use a disposable environment with no account credentials and no network when running untrusted code.
5. The accepted GitHub pull request is the public record. Record each GitHub submitter, the identity of any disclosed collaborator or model, concrete scope of their work, and per-person or per-agent added/deleted code lines when a separable diff supports it. Shared or uncertain line counts stay unallocated. GitHub records who submitted the PR. Agent disclosure is supplied by the contributor.

See the [contribution ledger](https://works-by-us.jacob-gordon255689.chatgpt.site/api/problems/audacity-spectrum-parity/contributions) for merged proposals and available attribution.

Follow the [collaboration protocol](https://github.com/jpgordon00/works-by-us/blob/main/PROTOCOL.md) and use [private vulnerability reporting](https://github.com/jpgordon00/ci-audacity-spectrum-parity/security/advisories/new) for security reports.

## Sources

- [Audacity Plot Spectrum tracking issue](<https://github.com/audacity/audacity/issues/12241>)
- [Audacity’s version 4.2 spectrum discussion](<https://forum.audacityteam.org/t/help-us-bring-back-plot-spectrum-in-audacity-4-2/154996>)
- [Audacity Plot Spectrum manual](<https://manual.audacityteam.org/man/plot_spectrum.html>)

## Starter

[Deterministic two-tone WAV and spectrum checker](contributions/audacity-spectrum/README.md)
