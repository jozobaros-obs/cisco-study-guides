# Cisco Certification Study Guides — Free Samples

A small static site that hosts **free sample chapters** of my Cisco certification
study guides, with links to the full books on Leanpub. Built for engineers
preparing for CCNP / CyberOps / DevNet-level exams who want to try before they buy.

🌐 **Live site:** https://jozobaros-obs.github.io/cisco-study-guides/

---

## 📚 Available guides

Each guide ships as a polished, exam-focused study book. Download the free PDF
sample to see the layout, depth, and style before purchasing the full version.

| Exam | Guide | Free sample | Full book |
|------|-------|-------------|-----------|
| 200-201 | CyberOps Associate (Cybersecurity) | [Sample PDF](./ccna-cybersecurity-sample.pdf) | _Leanpub_ |
| 350-201 | CBRCOR — CyberOps Professional Core | [Sample PDF](./cbrcor-sample.pdf) | [Leanpub](https://leanpub.com/cbrcor) |
| 350-901 | AUTOCOR | [Sample PDF](./autocor-sample.pdf) | _Leanpub_ |
| 300-435 | ENAUTO — Enterprise Automation | [Sample PDF](./enauto-sample.pdf) | _Leanpub_ |
| — | CCNA Automation | [Sample PDF](./ccna-automation-sample.pdf) | _Leanpub_ |

> **Note:** Replace each _Leanpub_ placeholder with the real book URL once you
> confirm the slug (only `cbrcor` is filled in). Leanpub slugs usually match the
> sample file name, e.g. `https://leanpub.com/autocor`.

---

## 🎯 What's inside the guides

- Exam-blueprint-aligned chapters, written for working engineers
- Real configuration examples (Cisco IOS / NX-OS, Python automation, NETCONF/RESTCONF)
- "Exam Tip", "Common Pitfall", and "From the Field" callouts
- End-of-chapter quizzes with answer keys
- Glossary and quick-reference back matter

---

## 🗂️ Repository structure

```
cisco-study-guides/
├── index.html                      # Landing page (the hub)
├── sitemap.xml                     # Sitemap submitted to Google Search Console
├── ccna-cybersecurity-sample.pdf   # 200-201 free sample
├── cbrcor-sample.pdf               # 350-201 free sample
├── autocor-sample.pdf              # 350-901 free sample
├── enauto-sample.pdf               # 300-435 free sample
├── ccna-automation-sample.pdf      # CCNA Automation free sample
└── README.md
```

---

## 🚀 How it's served

This is a **static site published with GitHub Pages**. There is no build step —
the files in the repository are served as-is.

- The site is published from this repository's Pages settings.
- Any push to the published branch redeploys automatically (usually within 1–2 minutes).
- To preview locally, just open `index.html` in a browser, or run a simple static
  server from the repo folder:

  ```bash
  python3 -m http.server 8000
  # then open http://localhost:8000
  ```

---

## 🔎 Search / indexing notes

- The site is verified in **Google Search Console** (URL-prefix property).
- `sitemap.xml` lists the hub plus each sample PDF and is submitted in Search Console.
- All `<loc>` entries must use the real domain `https://jozobaros-obs.github.io/...`
  (not a placeholder) and the file must be valid XML — one `<?xml ?>` declaration,
  one `<urlset>`, nothing before or after.
- New pages can be pushed into Google's priority crawl queue via **URL Inspection →
  Request Indexing**.

---

## ✍️ Author

**Jozef Baroš** — Network Architect & automation engineer.
Author of Cisco certification study guides and NetDevOps learning material.

- Leanpub: https://leanpub.com/u/ <!-- add your Leanpub author handle -->
- LinkedIn: <!-- add your LinkedIn profile URL -->

---

## 📄 License

The sample PDFs and book content are **© Jozef Baroš, all rights reserved**.
They are provided for personal evaluation only and may not be redistributed.

The site markup in this repository may be reused for reference.
