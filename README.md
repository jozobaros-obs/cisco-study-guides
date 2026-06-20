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
| 200-201 | CCNA Cybersecurity Learning Guide | [Sample PDF](./ccna-cybersecurity-sample.pdf) | [Leanpub](https://leanpub.com/ccna-cybersecurity)|
| 350-201 | CBRCOR Learning Guide | [Sample PDF](./cbrcor-sample.pdf) | [Leanpub](https://leanpub.com/cbrcor) |
| 350-901 | AUTOCOR Learning Guide | [Sample PDF](./autocor-sample.pdf) | [Leanpub](https://leanpub.com/autocor) |
| 300-435 | ENAUTO Learning Guide| [Sample PDF](./enauto-sample.pdf) | [Leanpub](https://leanpub.com/enauto) |
| 200-901 | CCNA Automation Learning Guide | [Sample PDF](./ccna-automation-sample.pdf) | [Leanpub](https://leanpub.com/ccna-automation) |
|   ---   | AI For Network Engineers | [Sample PDF](./AI_for_Network_Engineers_SAMPLE.pdf) | [Leanpub](https://leanpub.com/ai-network)) |

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
├── index.html                            # Landing page (the hub)
├── sitemap.xml                           # Sitemap submitted to Google Search Console
├── ccna-cybersecurity-sample.pdf         # 200-201 free sample
├── cbrcor-sample.pdf                     # 350-201 free sample
├── autocor-sample.pdf                    # 350-901 free sample
├── enauto-sample.pdf                     # 300-435 free sample
├── ccna-automation-sample.pdf            # CCNA Automation free sample
├── AI_for_Network_Engineers_SAMPLE.pdf   # AI for Network Engineers free sample
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

**ProDigitalJ** .

- Leanpub: [https://leanpub.com/u/](https://leanpub.com/u/prodigitalj) <!-- add your Leanpub author handle -->

---

## 📄 License

The sample PDFs and book content are **© ProDigitalJ, all rights reserved**.
They are provided for personal evaluation only and may not be redistributed.

The site markup in this repository may be reused for reference.
