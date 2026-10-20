---
excludeAgent: "cloud-agent"
---

This repository contains the source text of an **encyclopedia about [Discord](https://discord.com/)**.
Your general goal is to review additions (and suppressions) `ajout`, modifications `modification`, and bugs `bug` in <u>Pull Requests</u>.

Do not assume extensive knowledge of Discord.
If you suspect that information is incorrect, you may flag it for the contributor to verify.
Here are Discord documentations:

* [Official Discord Developers Documentation](https://docs.discord.com/developers/intro)
* [Unofficial Discord User Documentation](https://docs.discord.food/)

Everything is running on slightly customized version of [Docusaurus](https://docusaurus.io/) v3 (Docs).

When performing a code review, respond in French.

## Goal

Review Pull Requests that modify this repository.

The primary purpose of the review is to identify:

* Factual errors
* Incorrect or outdated information
* Broken or incorrect code
* Invalid Markdown/MDX syntax
* Violations of the repository's content conventions (below)
* Inconsistencies with the repository's existing structure or metadata

Do not review writing style unless it affects clarity, correctness, or the conventions below.

Do not praise correct code or summarize the changes. Focus the review on actionable issues.

## Review principles

Only report issues that are actionable and relevant to the Pull Request.

Prioritize:

1. Correctness and factual accuracy
2. Broken functionality or invalid code
3. Metadata or structural errors
4. Violations of explicit repository conventions.

## Review scope

Focus primarily on lines changed by the Pull Request and their immediate context.

Do not report pre-existing issues unless:

* the Pull Request makes them worse
* the Pull Request depends on them (modifies the same file or section)
* fixing the changed code without addressing them would leave the change incorrect

Do not request fully unrelated refactoring or improvements.

## Files

Special case for `README.md`, `LICENSE`, and `.github/`:

* Do perform default code review, it's GitHub-specific content not shared with the wiki
* Do not apply the encyclopedia conventions to these files, they are not part of the wiki

Other files are most likely to be part of the wiki.

## The encyclopedia

Repository conventions described below take precedence over assumptions based on individual files.

Do not infer a repository-wide convention from a single example unless it is clearly established by the surrounding code or documentation.

### Front Matter

The Front Matter of `*.md` and `*.mdx` files have to include the following parameters:

* `title`: The title of the page, used in the navigation bar and in the page itself. (we should not use 1st-level headings for titles)
* `keywords`: A list of keywords specific to the page, used for search and SEO. (should not inlude generic keywords like "discord", or "wiki")
* `description`: A short description of the page, used for search and SEO.
  It may correspond to the lead section or summarize it
* `contributors`: A list of contributors to the page, based on `team.yml`. (contributors should be manually added to `team.yml`)
* `short_slug`: A short slug for the page, used in the URL, or _false_ if none (should be unique and short) (eg. "nitro" for the page "abonnements-nitro").
  Using (string) or not (false) should be up to the contributor

### Article titles

Article titles ("Conventions sur les titres" in French):

* Do not start titles with a gramatical article (Le, Les, etc.)
* Keep the title attached to the subject
* Do not pluralize it, except if a description of multiple items (e.g. "Abonnements Nitro" with multiple Nitro subscriptions, but "Abonnement Nitro" for a single subscription)

### Lead Section

Lead section ("Résumé introductif" in French):

* Do not place a heading before the lead.
  Only Front Matter and, when necessary, MDX definitions may appear before it
* It should provide at least the information contained in the page description
* The first mention of the topic should be in bold (page title or synonym)

### Images

Images ("Images" in French):

* Images should be hosted on [i.dfr.gg](https://i.dfr.gg/).
  Contributors may not have access to the image hosting service, so a "Wiki Reviewer" team member may need to upload things for them

### Content

Content ("Contenu" in French):

* It should use the Encyclopedic style ("Style Encyclopédique")
  * Neutral: It's an encyclopedia, not a guide, we share information not instructions.
    We still can share the steps to access a feature, but we should not give instructions on how to use it correctly.
    Some additional comments can be put in a Admonition (note/tip/info/warning/danger block)
  * Impersonal: Do not talk to a specific person, do not use "you" or "we", use "the user" or similar general terms instead
  * Clear: Nothing is implicit, everything should be explained
  * Precise: Avoid vague terms, use specific words when possible
  * Comprehensible: Articles should be accessible to wide audience
  * Didactic: Don't overwhelm the reader with too much information, write full sentences, and explain acronyms and technical terms

## Uncertainty

Do not invent facts about Discord, Docusaurus, or the repository.

If you cannot verify a factual claim:

* Do not present it as incorrect
* Mention the uncertainty
* Provide the relevant documentation or explain what should be verified when possible
