# Publish Staging Workflow — Agent Instructions

When asked to **publish content from `staging/`**, execute the following steps *in order*.  
Do **not** skip or rearrange steps — consistency is critical for Jekyll compatibility.

---

## 🎯 Goal  
Turn all files in `staging/` into live blog posts (`_posts/`) and copy associated asset files (`.png`, `pdf`, etc.) to `assets/images/`.

---

- Familarize yourself with the repository structure by running `tree` from the git repository root.
- Follow existing conventions! German posts go to `_posts/`, English ones to `_posts/en`.
- As en example, look at the blog posts `_posts/2025-11-19-sccon.md` and `_posts/en/2025-11-19-sccon.md`.

For each main text file in staging:
- Determine the appropriate language (en or de) and the yyyy-mm-dd date (all date fields must be present).
  **ABORT** if anything cannot be determined!
- Choose an appropriate file name. Don't repeat dates (avoid 2020-12-31-convention-2020).
- Check whether the text contains any links that is not a sufficiently close match to an existing asset or those assets in the staging folder.
  So accept text where the corresponding assets can be identified with high confidence such that the links/references can be fixed.
  If any link cannot be resolved, then **ABORT**
- Copy the assets to /assets/images (do not overwrite existing ones!)
- Create the blog post text. Make sure to use use follow conventions regarding the file name and the meta data.
  - Make sure to appropriately set the metadata and fix any links.
  - For timestamps: If there is no specific mention of a time stamp, then use 10:00:00 as a default (avoid 00:00:00).
  - You may improve or fix formatting.
  - Don't alter the text itself, unless there are specific instructions for you (such as "please use this timestamp: 14:00"). Resolve such instructions, remove them from the text and note them in the final report.
- Create a corresponding translated version (update any links that need updating) of the blog post in the right folder:
  - German text needs to be placed into `_posts/`. The corresponding English translation needs to go to `_posts/en`.
  - Conversely, if the original text was English, it must have gone to `_posts/en` so the German translation goes to `_posts/`

Create a report of your actions:
- The created text files.
- Any instructions you encountered during processing and how to resolved them.
- The copied assets.
- The blog post metadata used
- Any encountered issues (if they are minor, auto-solve them)
- Any advices from your side

