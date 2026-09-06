# Tissue Tells the Truth — Manuscript Project

**Title:** *Tissue Tells the Truth: An Osteopathic Approach to Low Back Pain*  
**Subtitle:** How Osteopathic Medicine Uncovers the Real Causes the Medical System Misses  
**Author credit:** A Practicing Osteopath

This repository holds the working manuscript as Markdown files organized by front matter, numbered parts, chapters, and back matter. Tone throughout aims to be passionate but professional, mature, and non-adversarial—advocating collaboration between osteopathic and allopathic medicine rather than competition.

## File Structure

```
book/
├── README.md                          ← this file
├── front-matter/
│   ├── title-page.md                  ← title, subtitle, author, dedication, copyright, TOC
│   └── introduction.md                ← book introduction (when present)
├── part-i/                            ← Part I chapters (The Lie of “Non-Specific”)
├── part-ii/                           ← Part II chapters (Tissue Tells the Truth)
├── part-iii/                          ← Part III chapters (Finding the Cause)
├── part-iv/
│   ├── README.md                      ← Part IV introduction
│   ├── chapter-13-where-models-meet.md
│   ├── chapter-14-future-of-diagnosis.md
│   └── chapter-15-message-to-patients.md
└── back-matter/
    ├── glossary.md
    └── appendix.md
```

## How to Assemble the Manuscript

### Recommended reading / export order

1. `front-matter/title-page.md`
2. Part I chapters (in chapter number order), when present
3. Part II chapters, when present
4. Part III chapters, when present
5. `part-iv/README.md` (part introduction)
6. `part-iv/chapter-13-where-models-meet.md`
7. `part-iv/chapter-14-future-of-diagnosis.md`
8. `part-iv/chapter-15-message-to-patients.md`
9. `back-matter/glossary.md`
10. `back-matter/appendix.md`

### Concatenate to a single Markdown file (example)

From the `book/` directory:

```bash
# Adjust part-i/ii/iii paths as those chapters are added
cat front-matter/title-page.md \
  part-iv/README.md \
  part-iv/chapter-13-where-models-meet.md \
  part-iv/chapter-14-future-of-diagnosis.md \
  part-iv/chapter-15-message-to-patients.md \
  back-matter/glossary.md \
  back-matter/appendix.md \
  > /tmp/tissue-tells-the-truth-manuscript.md
```

### Pandoc (optional)

If Pandoc is installed, convert the assembled Markdown to DOCX or PDF for editing and review:

```bash
pandoc /tmp/tissue-tells-the-truth-manuscript.md -o Tissue_Tells_the_Truth.docx
```

### Word-count targets

| Component | Target |
|-----------|--------|
| Each full chapter | 3,500–4,500 words |
| Glossary | ~1,500–2,000 words |
| Appendix | ~2,500–3,500 words |
| Part introductions | Short framing essays |

Check counts with:

```bash
wc -w front-matter/*.md part-iv/*.md back-matter/*.md
```

## Editorial Notes

- Prefer full prose suitable for a trade / professional nonfiction audience.
- Preserve the book’s dual address: informed patients and clinicians.
- Keep medical claims careful: celebrate osteopathic specificity without dismissing acute medical or surgical excellence.
- Diagrams listed in the appendix are recommended for the published edition; they are described in text rather than embedded as binary assets in this Markdown workflow.
