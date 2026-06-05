Code for studying catastrophic forgetting in Whisper-based speech recognition using three adaptation strategies:

- Baseline – standard fine-tuning
- EWC – diagonal Fisher regularization
- mini-KFAC EWC – Kronecker-factored curvature approximation

**Datasets:** TEDLIUM (Stage A), Earnings22 (Stage B)  
**Model:** Whisper Small

## Usage
1.
```bash
pip install -r requirements.txt
```
2. Run all cells in `run.ipynb` (set `TARGET_SEED` as desired).
3. Results written to `runs/seed_<seed>/`.

## Evaluation
Task A WER (retention), Task B WER (adaptation), and Forgetting = Task\_A\_WER\_after − Task\_A\_WER\_before.