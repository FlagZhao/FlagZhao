# Website Updates Summary

## Date: November 13, 2025

This document summarizes all the updates made to your academic website based on your CV (cv.tex).

## Files Modified

### 1. `_pages/about.md`
**Status**: ✅ Updated

**Changes**:
- Replaced generic template text with your actual biography
- Added your research focus on GPU performance analysis, profiling, and optimization
- Included detailed research interests covering:
  - GPU Performance Analysis & Profiling
  - Memory System Optimization
  - Heterogeneous Computing
  - Compilation & Code Generation
- Added "Recent Highlights" section featuring:
  - SC 2025 paper acceptance (RedSan)
  - PNNL summer 2025 internship
  - Service roles (SPAA 2025 JPC, PPoPP 2025 AEC)
- Added comprehensive technical skills section

### 2. `_config.yml`
**Status**: ✅ Updated

**Changes**:
- Fixed name typo: "Yanbo ZHao" → "Yanbo Zhao"
- Updated bio: "4th Year Ph.D Student" → "4th-Year Ph.D. Student in Computer Science"
- Enhanced site description to include research focus
- Maintained all existing social media and academic profile links (Google Scholar, ORCID, GitHub)

### 3. `_data/navigation.yml`
**Status**: ✅ Simplified

**Changes**:
- Removed unnecessary navigation items (Portfolio, Blog Posts, Talks, Guide)
- Kept essential sections:
  - Publications
  - CV
  - Teaching
- Cleaner, more focused navigation

### 4. `_pages/cv.md`
**Status**: ✅ Completely Rewritten

**Changes**:
- Added link to PDF version of CV
- Updated Education section with accurate information:
  - Ph.D. at NC State (2022-Present)
  - M.S. at Shandong University (2019-2022)
  - B.S. at Shandong University (2015-2019)
- Updated Work Experience:
  - PNNL Research Intern (Summer 2025)
  - NCSU Teaching/Research Assistant (2022-Present)
- Added comprehensive Skills & Expertise section
- Added Service section with committee memberships
- Added Honors & Awards section
- Publications and Teaching sections automatically populated from collections

### 5. Publications (`_publications/`)
**Status**: ✅ New Files Created

**Deleted**:
- All 5 template publication files (2009-2025 examples)

**Created**:
1. `2025-11-redsan-sc.md`
   - Title: RedSan: Redundant Memory Instruction Sanitizer for GPU Programs
   - Venue: SC 2025
   - Status: Accepted, to appear
   - Full abstract and key contributions included

2. `2025-cuthermo-arxiv.md`
   - Title: cuThermo: Understanding GPU Memory Inefficiencies with Heat Map Profiling
   - Venue: arXiv Preprint
   - Status: Under Review
   - Full abstract and key contributions included

### 6. Teaching (`_teaching/`)
**Status**: ✅ Updated

**Deleted**:
- 2 template teaching files

**Created**:
- `2022-fall-csc246.md`
  - Course: CSC 246 - Operating Systems
  - Duration: Fall 2022 - Spring 2024
  - Detailed course description and responsibilities

## What Still Needs to Be Done (Optional)

### Optional Enhancements:

1. **Add Research Projects Section**
   - Could create a dedicated page for research projects from CV:
     - cuVein (ongoing)
     - HPC-in-Triton compilation bridge
     - Memogent
     - Cache persisting profiling tool

2. **Update/Remove Template Content**
   - Check `_talks/` directory - may contain template talks
   - Check `_portfolio/` directory - may contain template portfolios
   - Check `_posts/` directory - may contain template blog posts

3. **Add More Details to Publications**
   - Add paper links when available
   - Add BibTeX citations
   - Add preprint/arXiv links

4. **Profile Picture**
   - Ensure `images/profile.png` is your actual photo

5. **Social Media Links**
   - Consider adding LinkedIn profile
   - Consider adding Twitter/X if you have one

## How to Deploy

1. Commit all changes:
   ```bash
   git add .
   git commit -m "Update website with current CV information"
   ```

2. Push to GitHub:
   ```bash
   git push origin master
   ```

3. GitHub Pages will automatically rebuild your site (may take 1-2 minutes)

4. Visit your site at: https://flagzhao.github.io/FlagZhao

## Notes

- The PDF CV (`files/Yanbo_Zhao_CV_2025_Nov.pdf`) is already in the files directory and linked from the CV page
- All pages will automatically pull from the updated collections (publications, teaching)
- The site uses Jekyll and the Academic Pages template
- Configuration changes in `_config.yml` require a server restart if testing locally

## Testing Locally (Optional)

If you want to test the site locally before deploying:

```bash
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

---

**Summary**: Your academic website now accurately reflects your current research, publications, experience, and skills as documented in your CV. The site has been streamlined to focus on the most relevant sections for an academic profile.

