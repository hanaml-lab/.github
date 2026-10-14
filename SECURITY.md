# Security policy

This policy covers every repository under [github.com/hanaml-lab](https://github.com/hanaml-lab) that does not have
its own.

## Reporting a vulnerability

Please do not open a public issue. Report it privately, either through GitHub's
[private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)
("Report a vulnerability" on the repository's Security tab) or by email to
[info@hanaml.com](mailto:info@hanaml.com) with "Security" in the subject.

Include the repository and version or commit, what an attacker can do, and the steps or a proof of concept that
shows it. We acknowledge a report within three working days, keep you informed while we fix it, and credit you in
the advisory unless you ask us not to.

## What is in scope

- Code in these repositories, including bypasses of a permission rule, an approval or a budget in
  [hana-agents](https://github.com/hanaml-lab/hana-agents), which are security properties of that system.
- Model files we publish, where a file can execute code or does not match its published checksum.

Weaknesses of a model's behaviour (a jailbreak, a wrong answer) are not vulnerabilities; please open an issue on the
repository instead. Third-party dependencies are reported to their maintainers; tell us too if our use of one makes
it exploitable.

## Supported versions

The latest release of each repository receives fixes. Paper repos are frozen reference implementations of a paper
and receive fixes only for vulnerabilities.
