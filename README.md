# 💳Fake-Card-Analyzer
---

# Card Authenticity Detection using SSIM

This project detects whether a card is **real or fake** by comparing it with a reference image using the **Structural Similarity Index (SSIM)**.

### How SSIM works

* Both the reference card and the test card images are first **converted to grayscale**.
* SSIM compares small image patches and measures similarity in terms of:

  * **Luminance** (brightness)
  * **Contrast**
  * **Structure** (patterns and edges)
* The output is a **score between -1 and 1**:

  * **1.0 → Perfectly identical images**
  * **Close to 0 → Very different images**

### Why SSIM score is useful

* Unlike pixel-by-pixel comparison, SSIM focuses on **human visual perception**, making it more reliable for detecting small differences.
* A **high SSIM score** indicates the card is likely **real**, while a **low SSIM score** suggests the card is **fake**.
