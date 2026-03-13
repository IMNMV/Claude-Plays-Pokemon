# Claude Plays Pokemon Dataset

This repository contains a de-identified annotation dataset from a Claude Plays Pokemon chat corpus.

## Included File

- `pokemon_chat_annotations_anonymized.csv`: timestamped chat messages with channel metadata, raw message text, and binary annotation columns for gameplay events, chat behavior, model-state-related features, and anthropomorphization dimensions.

## Notes

- The direct `username` field has been removed.
- `message`, `time`, and `channel` are retained for context and replication, so this dataset should be treated as de-identified rather than fully anonymous.
- Annotation columns are binary indicators where `0` means absent and `1` means present.

## Column Groups

- Metadata: `time`, `channel`, `message`
- Gameplay events: battle outcomes, progress markers, encounters, item use, and related actions
- Model-state / reasoning tags: `Incorrect_Assumption`, `Stuck_In_Loop`, `False_Belief`, `Belief_Update`, and related variables
- Chat behavior tags: frustration, enthusiasm, encouragement, speculation, memes, directives, humor, and hints
- Anthropomorphization tags: cognitive, emotional, intentional, and social anthropomorphization

## Scope

- Rows: 107,145
- Format: CSV
- Intended use: descriptive analysis, annotation validation, and modeling of anthropomorphization in chat messages
