# Log

## 2026-11-10 baseline seed 0 (Track A)
- changed: starter recipe, all training photos, official budget 250,000, batch size 64
- why: baseline measurement of the starter configuration
- validation: 0.4965 (before: N/A)
- what it means: the starter recipe on all training photos gives a validation score of 0.4965; Tokyo easiest (0.638), Osaka hardest (0.341)

## 2026-11-10 baseline seed 1 (Track A)
- changed: same starter recipe, same selection, different random seed
- why: measure how much the score moves by chance when only the seed changes
- validation: 0.4924 (before: 0.4965)
- what it means: changing only the seed moves the score by about 0.004, which is the random variation between runs

## 2026-11-10 b1 (Track B)
- changed: starter train_b.py, ResNet18 at 224 px, 4 epochs, IMAGENET1K_V1 weights
- why: first Track B submission, to verify format and limits pass
- validation: 0.4987 (before: N/A)
- what it means: Track B b1 reaches 0.4987, within random variation of Track A; passes check_submission.py format and limits (11.17M parameters, 1.81B MACs, 44.7 MB)

No photo-curation or extra-photo experiment was performed. Both tracks used the starter configuration and all starter training photos only.
