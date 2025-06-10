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
Text-guided image editing, fueled by recent advancements in generative AI, is becoming increasingly widespread. This trend highlights the need for a comprehensive framework to verify text-guided edits and assess their quality. To address this need, we introduce EditInspector, a novel benchmark for evaluation of text-guided image edits, based on human annotations collected using an extensive template for edit verification. We leverage EditInspector to evaluate the performance of state-of-the-art (SoTA) vision and language models in assessing edits across various dimensions, including accuracy, artifact detection, visual quality, seamless integration with the image scene, adherence to common sense, and the ability to describe edit-induced changes. Our findings indicate that current models struggle to evaluate edits comprehensively and frequently hallucinate when describing the changes. To address these challenges, we propose two novel methods that outperform SoTA models in both artifact detection and difference caption generation.

## Citation
```bibtex
@inproceedings{yosef2025editinspector,
  title     = {EditInspector: A Benchmark for Evaluation of Text-Guided Image Edits},
  author    = {Yosef, Ron and Yanuka, Moran and Bitton, Yonatan and Lischinski, Dani},
  year      = {2025}
}
