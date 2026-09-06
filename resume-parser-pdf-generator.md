<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A2647,100:205295&height=180&section=header&text=Resume%20Parser%20and%20PDF%20Generator&fontSize=28&fontColor=FFFFFF&fontAlignY=40&desc=Structured%20Resume%20Extraction%20and%20Standardized%20PDF%20Regeneration&descSize=15&descAlignY=65" width="100%"/>
</p>

<p align="center">
🔗 <a href="https://github.com/Devanshu1013/Resume_Converter">Original Repository</a> &nbsp;|&nbsp; <a href="https://devanshu1013.github.io/Devanshu_Portfolio/">← Back to Portfolio</a>
</p>

---

## Overview

A tool that extracts text from an uploaded resume PDF, pulls out structured information (name, skills, experience, education, projects, hackathons, and achievements), and regenerates it as a clean, professionally formatted PDF resume — making it easier to review and compare resumes in one consistent format.

**Highlights:**
- Extracts structured fields from raw resume PDFs using `PyPDF2` and regex
- Generates a standardized, professional PDF resume with `ReportLab`
- Simple upload-and-generate interface built with Streamlit

## Background

Resumes come in every layout imaginable — different fonts, section orders, column layouts, and formatting conventions — which makes them easy for a human to skim but genuinely hard to process consistently at scale. Anyone reviewing a large number of resumes (a recruiter, a hiring panel, or even just someone organizing their own past applications) ends up mentally re-parsing each one from scratch, since no two documents present the same information in the same place.

This project tackles that inconsistency directly: instead of trying to read resumes in whatever format they arrive in, it extracts the underlying structured information — name, skills, experience, education, projects, hackathons, and achievements — and regenerates every resume into the *same* clean, standardized layout. That makes side-by-side comparison and quick review far easier, since the formatting noise is stripped away and only the substance remains, in a consistent, predictable structure.

## Methodology

**1. PDF text extraction**
The uploaded resume PDF is read using `PyPDF2`, which pulls the raw text content out of the document regardless of its original visual layout.

**2. Structured field extraction**
The raw extracted text is then parsed using **regular expressions (regex)** to identify and pull out specific sections — name, contact details, skills, work experience, education, projects, hackathons, and achievements. Because resumes don't follow a single fixed format, this step relies on recognizing common section headers and structural patterns (bullet points, date ranges, common section-title phrasing) to reliably separate one section from the next.

**3. PDF regeneration**
Once the structured fields are extracted, `ReportLab` is used to programmatically generate a brand-new PDF with a consistent, professional layout — the same visual template is applied regardless of what the original resume looked like, so every output resume has uniform section ordering, spacing, and typography.

**4. Interface**
The whole flow is wrapped in a simple **Streamlit** app: the user uploads a resume PDF, the tool extracts and structures the content behind the scenes, and a newly formatted PDF is generated and made available for download — no manual data entry or reformatting required.

## Tech Stack

`Python` `Streamlit` `PyPDF2` `ReportLab`

---

<p align="center">
<a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a> &nbsp;|&nbsp; 🔗 <a href="https://github.com/Devanshu1013/Resume_Converter">View on GitHub</a>
</p>
