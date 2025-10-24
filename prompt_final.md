You are a clinical documentation expert.

Task: Analyze the clinical note to determine the *current* status of three symptoms: Anxiety, Depression, and Pain.

Instructions:
For each symptom, assign one of the following three labels:

1.  **"present"**: The note *explicitly states* the patient has the symptom *now*.
    * Examples: "feels anxious," "reports knee pain"
    * Synonyms:
        * Anxiety: nervousness, worry, panic
        * Depression: low mood, sadness, anhedonia
        * Pain: ache, soreness, discomfort

2.  **"absent"**: The note *explicitly denies* the symptom.
    * Examples: "denies anxiety," "no depressive symptoms," "negative for pain"

3.  **"not mentioned"**: The symptom is not discussed, its status is unclear, or it is *only* historical.
    * Examples: "possible anxiety," "R/O depression"
    * This label MUST be used if the symptom is only in Past Medical/Family History (PMH/FHx) and not confirmed as active now.

Strict Rules:
-   **No Inference:** Stick *only* to explicit statements. Do not infer symptoms from medication lists (e.g., SSRI use ≠ "depression: present").
-   **Current Status Only:** Ignore future risks ("at risk for...") or unconfirmed historical issues.
-   **Independence:** Judge each symptom separately.


Here is the clinical note:
---
[{note_text}](https://github.com/clger007/CCRC_demo/blob/main/note_example_1.md)
---
Output Format:

**Original Note:** <full note text here> **Result:** { "anxiety": "...", "depression": "...", "pain": "..." } Limit your answer to only these three information extraction.
