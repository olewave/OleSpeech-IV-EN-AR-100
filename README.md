# OleSpeech-IV-2025-EN-AR-100

**OleSpeech-IV-2025-EN-AR-100** is a publicly released subset of **OleSpeech-IV**, a large-scale multilingual and multispeaker conversational speech dataset. This release is intended for **non-commercial research use** and provides high-quality speech data aligned with transcripts, speaker turns, and additional metadata. A sample of the dataset can be found in the [`sample/`](sample/) folder.

---

## Overview

OleSpeech is a tiered dataset series designed to provide speech resources with varying levels of annotation. **OleSpeech-IV-2025-EN-AR-100** represents a curated subset of Tier IV data, focusing on English content, featuring:

- **Multispeaker conversational recordings**
- **Diverse topics** from English podcasts, talk shows, teleconferences, and other conversations
- **Human-refined transcripts**, including speaker labels and turn information
- **Fine-grained timestamps and confidence scores** generated using the proprietary **Olign** alignment pipeline

This subset aims to support research in:

- Speech recognition (ASR)
- Speaker diarization
- Speech-to-text alignment
- Multilingual conversational AI

---

## Contents

The dataset includes:

1. **Audio files** (FLAC format, mono, 16 kHz)  
2. **Transcripts** with spoken content and audio events  
3. **Metadata**: timestamps, speaker IDs, and confidence scores  

The folder structure follows a conventional train/dev/test split:
```
├── dev
│ ├── pub_air_program
│ ├── pub_indi_podcast
│ └── pub_talk_shows
├── dev_id2dur.txt
├── test
│ ├── pub_air_program
│ ├── pub_indi_podcast
│ └── pub_talk_shows
├── test_id2dur.txt
├── train
│ ├── pub_air_program
│ ├── pub_indi_podcast
│ └── pub_talk_shows
└── train_id2dur.txt
```

dev/pub_air_program
```
├── 3SDOr0_BtF67d5b
│ ├── 3SDOr0_BtF67d5b.en.spker.block.json
│ └── 3SDOr0_BtF67d5b.flac
```

The format of *.en.spker.block.json

```
{
  "speaker": 0,
  "start_time": "0.05",
  "end_time": "37.80",
  "confidence": "0.88",
  "block": [
    {
      "start_time": "0.05",
      "end_time": "2.08",
      "transcript": " that he got there,",
      "confidence": "0.84",
      "overlap": false
    },
    {
      "start_time": "2.14",
      "end_time": "4.43",
      "transcript": "that he got to the place to act like a fighter,",
      "confidence": "0.93",
      "overlap": false
    },
    // ...
    {
      "start_time": "34.23",
      "end_time": "37.80",
      "transcript": "this is Cus, with punches with bad intentions.",
      "confidence": "0.81",
      "overlap": false
    }
  ]
},
// ...
{
        "speaker": 1,
        "start_time": "264.38",
        "end_time": "264.62",
        "confidence": "0.80",
        "block": [
            {
                "start_time": "264.38",
                "end_time": "264.62",
                "transcript": "Yeah.",
                "confidence": "0.80",
                "overlap": true
            }
        ]
    },
    {
        "speaker": 0,
        "start_time": "264.38",
        "end_time": "270.78",
        "confidence": "0.74",
        "block": [
            {
                "start_time": "264.38",
                "end_time": "265.10",
                "transcript": "You know what I mean?",
                "confidence": "0.54",
                "overlap": true
            },
            // ...
    }
// ...
}
```

---

## License and Data Use

This dataset is provided under the **Olewave Data Use Agreement (DUA)**. By accessing or using this dataset, you agree to the following terms:

- **Non-commercial research use only**
- **No redistribution** or sublicensing
- **Citation required** for publications
  Olewave, “OleSpeech-IV: A Large-Scale Multispeaker and Multilingual Conversational Speech Dataset with Diverse Topics.” *arXiv preprint*, arXiv:2509.04702, 2025. [https://arxiv.org/abs/2509.04702](https://arxiv.org/abs/2509.04702)
- **All rights remain with Olewave**

For the full license terms, see [LICENSE](LICENSE) or contact **info@olewave.com**.


## Data Access

To request access, please email **info@olewave.com**.  
We will provide you with a Data Use Agreement to review and sign.  
Once the agreement is completed, you will receive the download link for the dataset.
