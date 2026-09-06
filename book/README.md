# Tissue Tells the Truth — Manuscript Project

**Title:** *Tissue Tells the Truth: An Osteopathic Approach to Low Back Pain*  
**Subtitle:** How Osteopathic Medicine Uncovers the Real Causes the Medical System Misses  
**Author credit:** A Practicing Osteopath  
**Approximate length:** ~63,000 words

This repository holds the complete working manuscript as Markdown files organized by front matter, numbered parts, chapters, and back matter. Tone throughout aims to be passionate but professional, mature, and non-adversarial—advocating collaboration between osteopathic and allopathic medicine rather than competition.

**Central argument:** The label “Non-Specific Low Back Pain” is a failure of the current medical model, not a reflection of reality. Osteopathy offers a path to true specificity through palpation, clinical reasoning, and a holistic understanding of the body’s interconnected systems.

## File Structure

```
book/
├── README.md
├── FULL-MANUSCRIPT.md                 ← concatenated manuscript (generated)
├── front-matter/
│   ├── title-page.md
│   └── introduction.md
├── part-i/                            ← The Problem with “Non-Specific”
│   ├── README.md
│   ├── chapter-01-…
│   ├── chapter-02-…
│   └── chapter-03-…
├── part-ii/                           ← The Osteopathic Paradigm
│   ├── README.md
│   └── chapters 04–07
├── part-iii/                          ← The Clinical Reality
│   ├── README.md
│   └── chapters 08–12
├── part-iv/                           ← Bridging the Gap
│   ├── README.md
│   └── chapters 13–15
└── back-matter/
    ├── glossary.md
    └── appendix.md
```

## How to Assemble the Manuscript

### Recommended reading / export order

1. `front-matter/title-page.md`
2. `front-matter/introduction.md`
3. `part-i/README.md` then chapters 1–3
4. `part-ii/README.md` then chapters 4–7
5. `part-iii/README.md` then chapters 8–12
6. `part-iv/README.md` then chapters 13–15
7. `back-matter/glossary.md`
8. `back-matter/appendix.md`

### Concatenate to a single Markdown file

```bash
cat \
  book/front-matter/title-page.md \
  book/front-matter/introduction.md \
  book/part-i/README.md \
  book/part-i/chapter-*.md \
  book/part-ii/README.md \
  book/part-ii/chapter-*.md \
  book/part-iii/README.md \
  book/part-iii/chapter-*.md \
  book/part-iv/README.md \
  book/part-iv/chapter-*.md \
  book/back-matter/glossary.md \
  book/back-matter/appendix.md \
  > book/FULL-MANUSCRIPT.md
```

## Audience & Tone

Written for two audiences at once: (1) patients frustrated by the “non-specific” label, and (2) osteopaths, physiotherapists, and medical professionals seeking the osteopathic rationale. Clear, engaging prose; jargon explained when used; evidence referenced narratively (NICE, WHO, imaging research, OMT trials).

## Publishing Notes

- An invited foreword (respected osteopath, pain researcher, or former patient) is recommended for the published edition.
- Diagrams suggested for print: fascial lines, dermatomes, viscero-somatic reflexes, and flowcharts comparing the allopathic “rule-out” algorithm vs. the osteopathic “find-out” algorithm.
- Clinical cases are composite and anonymized for teaching; they are not identifiable patient records.
