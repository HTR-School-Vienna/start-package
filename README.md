# Handout: Publishing Ground Truth Data

## Part 1: File Preparation Checklist
Create a folder for your project and ensure it contains the following files and structure. Check the boxes as you complete them.

For collaborative writing of MD files you can use colab tool: https://chat.humanities.tools/. For formatting options of MarkDown (MD) see [MarkDown Guidelines](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax.).

- [ ] **`README.md`**
    *   **What is it:** The front page of your dataset.
    *   **Content:** Project name, description, license, and statistics.
    *   **File:** You can use this [template](README_TEMPLATE.md) and delete this file afterwards.
- [ ] **`CITATION.cff`**
    *   **What is it:** A specific file that tells services how to cite your data.
    *   **Content:** Authors, title, date, and DOI (once obtained).
    *   **Link to tool:** https://citation-file-format.github.io/
- [ ] **`htr-united.yml`** (or `.json`)
    *   **What is it:** Metadata file for the HTR-United catalog.
    *   **Content:** Script type, language, time period, and link to the data.
    *   **Link to tool:** https://htr-united.github.io/document-your-data.html
- [ ] **`guidelines.md`** (Optional but recommended)
    *   **What is it:** "Other documents" mentioned in the presentation.
    *   **Content:** Transcription rules used (e.g., how to handle abbreviations).
- [ ] **Data Folder: `images/`**
    *   **Content:** Your high-resolution manuscript images (JPG/PNG/TIFF).
- [ ] **Data Folder: `page/`** (or `alto/`)
    *   **Content:** The XML transcription files corresponding to the images.
---

## Part 2: Organize Your Files
Separate your data into two distinct groups on your computer.

### Group A: Lightweight Files (For GitHub)
*These files verify the structure and provide the transcriptions.*
- [ ] **`README.md`** (Project overview)
- [ ] **`CITATION.cff`** (Citation metadata)
- [ ] **`htr-united.yml`** (Catalog metadata)
- [ ] **`guidelines.md`** (Transcription rules)
- [ ] **`page/`** or **`alto/`** folder (Contains only `.xml` transcription files)

### Group B: Heavyweight Files (For Zenodo)
*These files are too large for GitHub.*
- [ ] **`images.zip`** (A compressed folder containing all manuscript images: JPG/TIFF/PNG)


---

## Part 3: Publishing Workflow Checklist

Follow these steps in order to link the two platforms.

### Step 1: Upload to Zenodo (Images)
- [ ] Go to [zenodo.org](https://zenodo.org) -> "New Upload".
- [ ] Drag & drop your **Group B** files (`images.zip`).
- [ ] Fill in the basic info (Title, Authors).
- [ ] **Important:** Click "Reserve DOI" (do not publish yet).
- [ ] **Copy the Reserved DOI** (e.g., `10.5281/zenodo.1234567`).

### Step 2: Upload to GitHub (Transcriptions)
- [ ] Paste the Zenodo DOI into your `README.md` and `CITATION.cff` files (see templates below).
- [ ] Create a New Repository on GitHub.
- [ ] Upload **Group A** files to this repository.
- [ ] Copy the **GitHub Repository URL**.

### Step 3: Finalize Zenodo
- [ ] Go back to your Zenodo upload page.
- [ ] In the "Related/Alternate Identifiers" section, add the **GitHub Repository URL**.
- [ ] Click **Publish**.

### Step 4: HTR-United (Cataloging)
- [ ] Copy the link to your `htr-united.yml` file on GitHub.
- [ ] Send me the link to file via Discord or email martin.rocek@ff.cuni.cz
