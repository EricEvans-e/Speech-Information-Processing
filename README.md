# Speech Information Processing Course Materials

This directory is organized by course scope first, then by lab.

## Directory Map

- `00_course_overview/` - course opening slides, grading policy, and overall course/project notes.
- `01_lectures/` - theory lecture slides grouped by topic.
  - `01_intro/` - signal processing and introductory material.
  - `02_machine_learning/` - probability, GMM/EM, and HMM lectures.
  - `03_deep_learning/` - language modeling, RNN, conditioned generation, and attention lectures.
  - `04_asr/` - ASR lecture slides.
  - `05_tts_and_speaker/` - TTS and speaker-recognition experiment lecture decks.
- `02_labs/` - working lab materials, notebooks, transcripts, manuals, code, and lab datasets when bundled with a lab.
  - `lab1_signal_features/` - speech signal processing, spectrograms, FBank/MFCC, and optional pretrained audio features.
  - `lab2_poetry_lstm/` - PyTorch/LSTM poetry generation.
  - `lab3_facodec_disentanglement/` - FACodec speech discretization, feature disentanglement, reconstruction, and voice conversion.
  - `lab4_tts_melotts/` - MeloTTS speech synthesis transcripts, instructions, and the cloned `MeloTTS-Homework/` assignment repository.
  - `lab5_speaker_recognition/` - ECAPA-TDNN speaker-recognition notebooks and AISHELL mini data bundled with the lab.
- `03_archives/` - original compressed packages and duplicate extracted originals.
  - `zip_originals/` - original `.zip` downloads.
  - `extracted_originals/` - duplicate extracted copies kept for provenance.
  - `macos_metadata/` - `__MACOSX` and `.DS_Store` metadata preserved from zip extraction.
- `04_datasets_and_models/` - shared datasets or model resources not tied to a single working lab folder.
  - `poetry_data/` - Chinese poetry JSON dataset extracted from `data.zip`.
  - `facodec_model/` - currently empty; reserved for standalone FACodec model assets if they are separated later.
  - `aishell_mini/` - currently empty; Lab 5's working AISHELL mini copy is under `02_labs/lab5_speaker_recognition/data/`.
- `99_notes/` - reserved for future notes and summaries.

## Common Entry Points

- Lab 1 notebook: `02_labs/lab1_signal_features/exp1_2026.ipynb`
- Lab 2 notebook: `02_labs/lab2_poetry_lstm/lab2.ipynb`
- Lab 3 FACodec guide: see the experiment-guide PDF in `02_labs/lab3_facodec_disentanglement/`
- Lab 4 MeloTTS homework repo: `02_labs/lab4_tts_melotts/MeloTTS-Homework/`
- Lab 5 notebooks: `02_labs/lab5_speaker_recognition/01_setup.ipynb`, `02_labs/lab5_speaker_recognition/02_speaker_embedding.ipynb`, and `02_labs/lab5_speaker_recognition/03_asv_asi.ipynb`

## Lab Count

The confirmed lab set is:

1. Lab 1 - speech signal processing and acoustic features.
2. Lab 2 - LSTM poetry generation.
3. Lab 3/4 numbering conflict - FACodec speech discretization and disentanglement. The meeting note calls it the third experiment, while the manual title says experiment four.
4. Lab 4 - MeloTTS speech synthesis.
5. Lab 5 - speaker recognition.

There are 19 graded lab sub-items across these materials: 17 required items and 2 bonus items. The course overview also mentions a separate team Project track.
