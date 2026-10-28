# LazyCats

Welcome to **LazyCats**! We are an open-source development group building browser extensions and tools designed to make creating, posting, and enjoying fanworks on [Archive of Our Own (AO3)](https://archiveofourown.org) smoother and more accessible.

> _**Disclaimer:** LazyCats and its projects are unofficial community creations and are not affiliated with, endorsed by, or supported by the Organization for Transformative Works (OTW) or Archive of Our Own (AO3). Please do not direct questions or bug reports about these tools to AO3 support._

---

## AO3 Podfic Posting Helper

The **AO3 Podfic Posting Helper** streamlines your workflow when posting a podfic to Archive of Our Own by importing metadata—such as tags, ratings, relationships, characters, and work summaries—directly from the original text work into the AO3 new work form.

![AO3 Podfic Posting Helper Screenshot](https://raw.githubusercontent.com/LazyCats-dev/ao3-podfic-posting-helper/main/images/pop-up-screen-shot.png)

### Download & Install

<a href="https://chrome.google.com/webstore/detail/ao3-podfic-posting-helper/liceoplaldpcfdkndimfppgdcbophgma?utm_source=github&utm_medium=web&utm_campaign=github_pages"
    target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/chrome-logo.svg" class="logo">
    Chrome Web Store
</a>
<a href="https://addons.mozilla.org/en-US/firefox/addon/ao3-podfic-posting-helper/" target="_blank" rel="noopener"
    class="button">
    <img alt="" role="presentation" src="/assets/img/firefox-logo.svg" class="logo">
    Firefox Add-ons Store
</a>
<a href="https://microsoftedge.microsoft.com/addons/detail/ao3-podfic-posting-helper/bhggifekpnmhgpnpgngnfkfjdehlfaoj" target="_blank" rel="noopener"
    class="button">
    <img alt="" role="presentation" src="/assets/img/edge-logo.svg" class="logo">
    Microsoft Edge Add-ons
</a>
<a href="https://github.com/LazyCats-dev/ao3-podfic-posting-helper" target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/github-logo.png" class="logo"> Source & Releases
</a>

### Usage

#### Filling in the New Work Form

1. Navigate to the [New Work form](https://archiveofourown.org/works/new) on AO3.
2. Click the extension icon in your browser toolbar.
3. Set the **"URL of work to import from"** field to the URL of the work you are podficcing.
4. Click **"Import"**.
5. Fields in the New Work form will be automatically populated with the metadata from the source work.

#### Advanced Options & Custom Templates

The extension supports custom templates for the title, summary, and work text fields:

1. Click the extension icon in your browser toolbar.
2. Click the **gear icon** in the top right corner to open the options page.
3. Configure your desired template for each field.
4. Click the **"Save"** button on each template you modify.
5. When importing, select **"Custom"** from the corresponding drop-down to use your saved template.

### Community & Resources

* [Infomercial: The AO3 Podfic Posting Helper (blackglass, esbielle, LittleRedRobinHood, Ravin, TheLordOfLaMancha)](https://archiveofourown.org/works/44137485)
* [Contributing Guide](https://github.com/LazyCats-dev/ao3-podfic-posting-helper/blob/main/CONTRIBUTING.md)
* [Report an Issue](https://github.com/LazyCats-dev/ao3-podfic-posting-helper/issues/new)

### Credits

Created and maintained by:

* [irrationalpie](https://archiveofourown.org/users/irrationalpie/pseuds/irrationalpie)
* [Jeremy Mowery](https://mowery.dev)
* [lastontheboat](https://archiveofourown.org/users/lastontheboat)

---

## AO3 Accessibility Helper

The **AO3 Accessibility Helper** is a lightweight, zero-permission Manifest V3 browser extension for Chrome, Firefox (Desktop & Android), and Microsoft Edge that checks your work HTML on Archive of Our Own for common accessibility barriers before you post.

When you open AO3's Post New Work, Edit Work, Add Chapter, or Edit Chapter page, the extension embeds an **AO3 Accessibility Check** panel directly beneath the work text HTML editor. As you write or paste HTML, it highlights issues in real time and lets you jump directly to the offending line with a single click.

![AO3 Accessibility Helper Screenshot](https://raw.githubusercontent.com/LazyCats-dev/ao3-a11y-helper/main/docs/screenshot.png)

### Links & Source

<a href="https://github.com/LazyCats-dev/ao3-a11y-helper" target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/github-logo.png" class="logo"> GitHub Repository
</a>
<a href="https://github.com/LazyCats-dev/ao3-a11y-helper/issues" target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/github-logo.png" class="logo"> Report an Issue
</a>

### Key Checks & Features

Because AO3 sanitizes HTML and strips custom `aria-*` attributes, all accessibility checks are tailored specifically to AO3's permitted HTML subset:

* **Images:** Flags `<img>` tags missing `alt` attributes or using suspicious placeholder/filename text.
* **Scene Breaks:** Identifies unformatted text scene breaks (such as `***` or `---`) that screen readers read aloud awkwardly, encouraging semantic horizontal rules (`<hr>`).
* **Heading Hierarchy:** Catches empty headings and skipped heading levels (e.g. `<h3>` without an `<h2>`).
* **Link Clarity:** Flags empty links and ambiguous phrases (such as "click here" or "link").
* **Fragile Image Hosting:** Detects temporary or fragile hosting URLs (such as Discord CDN links) that expire and break over time.
* **Formatting Best Practices:** Warns about chained `<br><br>` tags used instead of proper `<p>` paragraph tags, inaccessible `<table>` markup missing headers or captions, unlabeled `<details>` disclosure elements, and obsolete presentation tags (`<center>`, `<font>`, `<strike>`).
* **One-Click Jump:** Provides a **"Highlight in HTML"** button on each warning to instantly focus and highlight the line in your editor.
* **Zero Permissions & Private:** Operates with no special browser permissions (`permissions: []`). Runs 100% locally in your browser—no drafts, text, or personal data ever leave your device.

---

## Community & Support

Have questions, suggestions, or want to get involved with LazyCats projects?

<a href="https://discord.gg/rhynWjrCw2" target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/discord-logo.svg" class="logo"> Discord Server
</a>
<a href="https://github.com/LazyCats-dev" target="_blank" rel="noopener" class="button">
    <img alt="" role="presentation" src="/assets/img/github-logo.png" class="logo"> LazyCats on GitHub
</a>
