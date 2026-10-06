# Contributing to Unit 404 (CDIV)

Thank you for helping. This guide is the default for every public repository in the `unitCDIV` organisation. A repository may add its own `CONTRIBUTING.md` with extra detail.

Everyone who takes part agrees to the [Code of Conduct](CODE_OF_CONDUCT.md).

## The curriculum site

The source of the curriculum site, [unitcdiv.fairytale.ai](https://unitcdiv.fairytale.ai/), is maintained in a private repository. You can still shape it:

| You want to… | Do this |
|:--|:--|
| Report a factual error or unclear explanation | [Open a *Content error* issue](https://github.com/unitCDIV/.github/issues/new/choose) and quote the page URL and the passage |
| Report a broken link or a page that doesn't work | Open a *Broken link or site bug* issue |
| Write or review a lesson | Open a *Lesson proposal* issue first, so we can agree on scope before you write |
| Report a security problem with the site | **Don't open an issue.** Follow the [security policy](SECURITY.md) |

Maintainers turn accepted reports and proposals into site changes. Lesson authors are credited on the lesson page and in the release notes.

### What a good lesson proposal includes

- The course (for example `CDIV-F101`) and the lesson from its syllabus.
- Three learning objectives, each starting with a verb.
- The worked example you plan to use, and the exercise that adds to the course artifact.
- For an Offensive (`CDIV-X`) lesson: how the exercise runs entirely inside the reader's own isolated lab.

## Public tool and lab repositories

Repositories such as labs and tools accept pull requests.

1. **Open an issue first** for anything bigger than a typo, so effort isn't wasted.
2. **Fork, branch and keep changes focused**: one change per pull request.
3. **Explain what and why** in the pull request description, and how you tested it.
4. **Sign off your commits** (`git commit -s`) to confirm you have the right to contribute the work under the repository's licence.

## Offensive content policy

This applies to every contribution, in every repository. Contributions that break it will not be merged.

1. **Authorized use only.** Material must state that techniques may only be applied with the system owner's written permission.
2. **Lab targets only.** Exercises and examples target disposable environments the reader provisions and controls: local containers on an isolated network, or VMs on an internal or host-only network.
3. **No live third-party targets.** No real hosts, domains or IP addresses that the reader doesn't own. Use reserved names (`*.example`, `*.test`, `*.invalid`, `localhost`, `example.com`) and documentation addresses (`192.0.2.0/24`, `198.51.100.0/24`, `203.0.113.0/24`, `2001:db8::/32`), or private lab ranges.
4. **Never expose vulnerable systems.** Lab configurations must not publish deliberately vulnerable services beyond `127.0.0.1` or an isolated network.
5. **Reports, not trophies.** Frame findings by severity, evidence and remediation.

## Licences

- **Lessons and other written content**, including the code samples in lessons: [CC BY-NC 4.0](LICENSE-CONTENT). Non-commercial reuse with credit.
- **The curriculum site's own code** (HTML, CSS, JavaScript, templates and tooling): proprietary, all rights reserved.
- **Code in public tool and lab repositories**: [MIT](LICENSE), unless a repository says otherwise.

By contributing, you agree that your contribution is licensed under the same terms as the material you contribute to: CC BY-NC 4.0 for lesson content, and the repository's licence for code. Contributions that end up in the curriculum site's own code stay all rights reserved, and you grant Fairytale the right to use them. Sign off your commits (`git commit -s`) to confirm you have the right to contribute the work.
