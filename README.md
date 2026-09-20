# Sami Karam 👋

**AI systems + Cybersecurity | CS Co-op @ Concordia | Research Intern, Polytechnique Montréal (Summer 2026)**

Third-year Computer Science co-op student at Concordia. I build and evaluate machine learning and LLM systems. Most of my recent work is on agentic AI and on checking whether model results hold up.

## 🔬 Research

**Research Intern, Polytechnique Montréal** · May – Aug 2026
Applied machine learning research in cybersecurity on Prof. Adel Abusitta's team, joint work with one co-author. Recipient of the 2026 Undergraduate Summer Internship Award (1 of 12 from 326 applicants across 36 Canadian universities). Manuscript in preparation.

* Built a streaming pipeline over host telemetry from the DARPA OpTC public dataset, roughly 1.1 TB across about 1,000 enterprise hosts, aggregating tens of millions of host event records into 42,896 clean per-process activity trees used as a fixed reference set.
* Audited a malware family classifier reporting 0.79 accuracy and found 40.5% of its test set were near-duplicate repacks of training samples, using TLSH fuzzy hashing. Rebuilt the data split so near-duplicate groups never span both training and test, which put the honest baseline at 0.63 and reset the project's target.
* Ran a stratified LLM-as-judge audit of 2,084 cluster interpretations across the 25 largest of 277 clusters, sampling equally across five membership-strength bands, and measured a 0.106 coverage decline from cluster cores to boundaries with non-overlapping confidence intervals. Validated the judge with a negative control that re-judged every document under a deliberately wrong cluster name, establishing 0.686 discrimination and a 0.000 both-endorsed rate.
* Surfaced an Empire agent masquerading as `csrss.exe` sitting at full membership strength in a benign cluster core and endorsed by the judge, showing that automated cluster descriptions have to be treated as hypotheses rather than evidence.
* Built a verification script that re-runs every check a fresh clone can reproduce, and tied each reported figure to a tracked artifact so any number traces back to the run that produced it.

`Python` `Linux` `scikit-learn` `HDBSCAN` `TLSH` — lab repository is proprietary and not shared.

## 🛠 Projects

* **Brim Expense Intelligence.** 1st place, Brim Financial Challenge @ MPC Hacks 2026 (193 participants, 24h). An agentic AI co-pilot that audits corporate-card spend against policy. A multi-step agent runs its own read-only database queries before judging each charge, so every dollar figure is query-derived rather than model-generated. Built with a teammate on a demo dataset. `React` `Node.js` `MongoDB` `Anthropic API` · [live demo](https://brim-expense-intel.onrender.com/) · [video](https://www.youtube.com/watch?v=VsVfb5BQReM&feature=youtu.be)

* **Smart Course Companion.** Course and GPA tracking web app (SOEN 287, team of 4, graded 10/10). I built the server foundation and the authentication backend: Express 5 with routes, controllers, models and middleware, SQLite through Sequelize, bcrypt-hashed passwords and JWT, and the auth middleware behind every protected route of a 26-endpoint API. `JavaScript` `Node.js` `Express` `SQLite` `Sequelize` (code private under course policy)

* **CNN Skin-Lesion Classification.** PyTorch pipeline benchmarking ResNet-50, MobileNetV2 and VGG-16 across three dermoscopic datasets (HAM10000, ISIC 2019, SkinDS; 4, 8 and 14 classes; 49,198 images total) under identical hyperparameters, with stratified zero-overlap splits. Gradual-unfreeze transfer learning reached 89.29% accuracy and 0.763 macro-F1 on HAM10000, up 5.5 points over training from scratch, with minority classes gaining most. Diagnosed VGG-16's majority-class collapse hidden behind 77.3% accuracy (macro-F1 0.218, zero minority recall) and recovered it to 84.45%. MobileNetV2 matched ResNet-50 on macro-F1 across 14 classes at 10x fewer parameters. `PyTorch` `scikit-learn` `NumPy` (COMP 472, graded A-; code private under course policy)

* **[Java Technical Portfolio](https://github.com/Meartops/Java-Technical-Portfolio).** Algorithmic efficiency and cache-locality exercises in Java.

## 💻 Stack

* **ML & data:** Python, PyTorch, scikit-learn, NumPy, pandas
* **AI systems:** LLM agent tool loops, Anthropic Messages API, prompt engineering, schema-constrained decoding, LLM-as-judge evaluation
* **Full-stack:** JavaScript, React, Node.js, Express, MongoDB, SQLite, REST API design
* **Languages & tools:** Java, C, Bash, Git, Linux (Ubuntu), Docker, JUnit, pytest

## 📌 Also

* GPA 3.33 / 4.30 · Trilingual (English, French, Arabic)
* [LinkedIn](https://linkedin.com/in/karamsami)
