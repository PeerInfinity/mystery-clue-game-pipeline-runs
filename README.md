# Mystery clue game: the pipeline's run records

An archive. These are the records of the runs of the new-story pipeline of
[mystery-clue-game](https://github.com/PeerInfinity/mystery-clue-game) (its `v2/pipeline/`, itself archived there):
for each run, every step's inputs, the model's replies and the files made from them. They were kept in that
repository under `v2/pipeline/runs/` until 2026-11-25 (its commit `81582f6`), and moved here so that the game can be
taken as a submodule without them. Nothing in the game reads them.

| Folder | What it is |
|---|---|
| `silver-blaze/`, `silver-blaze-r2/` | The two runs of the pipeline on "Silver Blaze" |
| `speckled-band/` | The run on "The Speckled Band" |
| `silver-blaze-8b/`, `silver-blaze-9b-groups/`, `silver-blaze-9b-scenes/`, `silver-blaze-9b-whole/` | Trials of single steps |

**Spoilers:** these records give away both stories.

To use the archived pipeline again, clone this repository into the game's tree as `v2/pipeline/runs`
(`git clone https://github.com/PeerInfinity/mystery-clue-game-pipeline-runs v2/pipeline/runs`): the pipeline's
scripts read and write a run's folder there (`v2/pipeline/README.md` in the game). The prompts as sent and each
run's assembled case are not kept: the pipeline's own scripts rebuild them.

The history of these files before the move is in the game's repository.
