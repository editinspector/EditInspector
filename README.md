# EditInspector — Benchmark for Text-Guided Image-Edit Evaluation

## Benchmark Files
- **`benchmark/editinspector_benchmark.csv`** – 783 human-annotated MagicBrush edits  
- **`benchmark/imagen3_100_benchmark.csv`** – 100 human-annotated Imagen3 edits  
- **`benchmark/ultraedit_100_benchmark.csv`** – 100 human-annotated UltraEdit edits  
- **`benchmark/editinspector_100_benchmark.csv`** – 100 human-annotated MagicBrush edits

## Pipeline & Code
- **`EditInspector Pipeline.ipynb`** – full pipeline for  
  - main-difference caption generation  
  - artifact detection methods  
  - data-augmentation methods  

## Experiments
- **`experiments/`** notebooks for  
  - evaluating models on EditInspector Yes/No questions  
  - difference-caption generation evaluation  
  - running the fine-tuned model (**`EditInspector - Finetune Model Example.ipynb`**)  

## Training Data
- **`train_data/`** – 31 059 augmented training instances created by  
  1. **Negative-edit augmentation** (deceptive target objects)  
  2. **Reverse-direction augmentation** (flip add/remove/replace/attribute edits)  

## Abstract
Text-guided image editing is widespread, yet verifying edits is still hard. **EditInspector** provides a five-dimension benchmark (accuracy, artifacts, technical precision, contextual consistency, change description). It contains nearly 1 000 annotated edits, a zero-shot caption pipeline that doubles SoTA main-difference accuracy, a 64 %-accurate artifact detector, and a fine-tuned LLaVA model matching larger VLMs at lower cost.

## Citation
```bibtex
@inproceedings{yosef2025editinspector,
  title     = {EditInspector: A Benchmark for Evaluation of Text-Guided Image Edits},
  author    = {Yosef, Ron and Yanuka, Moran and Bitton, Yonatan and Lischinski, Dani},
  year      = {2025}
}
