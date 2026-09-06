# Tissue Tells the Truth, Manuscript Project

**Title:** *Tissue Tells the Truth*
**Subtitle:** An Osteopathic Approach to Low Back Pain
**Author credit:** A Practicing Osteopath
**Approximate length:** ~64,000 words

This repository holds the complete working manuscript as Markdown files organized by front matter, numbered parts, chapters, and back matter. Tone throughout aims to be passionate but professional, mature, and non-adversarial, advocating collaboration between osteopathic and allopathic medicine rather than competition.

**Central argument:** The label “Non-Specific Low Back Pain” is a failure of the current medical model, not a reflection of reality. Osteopathy offers a path to true specificity through palpation, clinical reasoning, and a holistic understanding of the body’s interconnected systems.

## File Structure

```
book/
├── README.md
├── FULL-MANUSCRIPT.md          ← concatenated manuscript (generated)
├── exports/
│   └── Tissue-Tells-the-Truth.pdf
├── front-matter/
│   ├── title-page.md           ← title, dedication, copyright, TOC
│   ├── foreword-placeholder.md
│   └── introduction.md
├── part-i/                     ← Part I, The Problem with “Non-Specific”
│   ├── README.md
│   ├── chapter-01-the-diagnosis-that-means-nothing.md
│   ├── chapter-02-the-allopathic-formula.md
│   └── chapter-03-the-red-flag-dilemma.md
├── part-ii/                    ← Part II, The Osteopathic Paradigm: A Philosophy of Specificity
│   ├── README.md
│   ├── chapter-04-structure-governs-function.md
│   ├── chapter-05-the-body-is-a-unit.md
│   ├── chapter-06-self-healing-mechanisms.md
│   └── chapter-07-five-models.md
├── part-iii/                   ← Part III, The Clinical Reality: No Formula, Only Principles
│   ├── README.md
│   ├── chapter-08-the-art-of-palpation.md
│   ├── chapter-09-case-studies-biomechanical.md
│   ├── chapter-10-case-studies-visceral-neuro.md
│   ├── chapter-11-the-failed-protocol.md
│   └── chapter-12-the-toolkit.md
├── part-iv/                    ← Part IV, Bridging the Gap: A Vision for Integrated Care
│   ├── README.md
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
2. `front-matter/foreword-placeholder.md`
3. `front-matter/introduction.md`
4. `part-i/README.md` then chapters 1–3
5. `part-ii/README.md` then chapters 4–7
6. `part-iii/README.md` then chapters 8–12
7. `part-iv/README.md` then chapters 13–15
8. `back-matter/glossary.md`
9. `back-matter/appendix.md`

### Concatenate to a single Markdown file

```bash
cat \
  book/front-matter/title-page.md \
  book/front-matter/foreword-placeholder.md \
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

(Chapter filenames are zero-padded, so shell glob order matches reading order.)

## Audience & Tone

Written for two audiences at once: (1) patients frustrated by the “non-specific” label, and (2) osteopaths, physiotherapists, and medical professionals seeking the osteopathic rationale. Clear, engaging prose; jargon explained when used; evidence referenced narratively (NICE, WHO, imaging research, OMT trials).

## Publishing Notes

- An invited foreword (respected osteopath, pain researcher, or former patient) is recommended for the published edition; see `front-matter/foreword-placeholder.md`.
- Diagrams suggested for print: fascial lines, dermatomes, viscero-somatic reflexes, and flowcharts comparing the allopathic “rule-out” algorithm vs. the osteopathic “find-out” algorithm.
- Clinical cases are composite and anonymized for teaching; they are not identifiable patient records.
