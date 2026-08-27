# Goal Description
We will update the existing LaTeX résumé to improve visual hierarchy and adopt a modern, minimal, sans-serif aesthetic, honoring the exact wording and content from the original `sample.md`. We will enhance typography, introduce structural indentation for clarity, redesign the Education section's layout, and refine line spacing.

## User Review Required
Please review the proposed styling and let me know if you approve or require any tweaks before I modify the LaTeX code.

## Proposed Changes

### 1. Typography and Global Layout (`preamble.tex`)
- **[MODIFY]** `preamble.tex`: 
  - Switch the entire document to a clean, modern sans-serif typeface (e.g., Helvetica via `\usepackage{helvet}` and `\renewcommand{\familydefault}{\sfdefault}`).
  - Add the `changepage` package to enable clean, block-level indentation (`adjustwidth` environment) without using colored boxes or tabular environments.

### 2. Project Hierarchy and Indentation (`sections/projects.tex`)
- **[MODIFY]** `projects.tex`:
  - Enhance project titles: Use `{\large \textbf{ProjectName}}` flush with the left margin.
  - Subordinate dates: Keep them right-aligned on the same line, but slightly smaller and italicized `{\small \textit{Date}}`.
  - Indentation: Wrap the subtitle, stack, and bullet points in an `adjustwidth` environment (e.g., indented by `0.15in`) so they are visually grouped under the title.

### 3. Education Redesign (`sections/education.tex`)
- **[MODIFY]** `education.tex`:
  - Strong institution name: Flush left and bold `{\large \textbf{Institution}}`.
  - Subordinate metadata: Wrap the degree, expected date, and GPA in an `adjustwidth` environment (indented beneath the institution).
  - Degree left-aligned and italicized.
  - Expected graduation date placed on the right side of the degree line, italicized.
  - GPA / Semester line placed immediately beneath the degree.

### 4. Skills Formatting and Spacing (`sections/skills.tex`)
- **[MODIFY]** `skills.tex`:
  - Maintain the category line format.
  - Introduce minimal, precise line spacing between the lines (e.g., `\\[2pt]`) to keep them cleanly grouped without looking crowded. 

## Verification Plan
### Manual Verification
- I will execute the implementation plan.
- You will compile the project (`pdflatex main.tex`) to visually inspect the PDF, ensuring a minimalist, highly structured, clean white technical resume.
