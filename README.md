# LoRA-LA: Low-Rank Atom Distillation for Efficient Segmentation

This repository contains the training notebook, logs, and results for our paper:

**"Efficient Student Segmentation: Reducing Linear Layer Computations with Near-Teacher Accuracy"**  
_Aleksandr Druzhinin, 2025_

Preprint: (arXiv link coming soon)  
Checkpoints and logs: https://drive.google.com/drive/folders/1Eotm6cXJR0BU6kmUFpOaJP4Tn5lkPoGW?usp=drive_link

---

## 🔥 Highlights
- **Teacher**: SegFormer-B0 for binary human segmentation.
- **Student**: trained with **LoRA-LA (Low-Rank Atom + Delayed Sparsity + KR-hard + EMA)**.
- **Results**:
  - Teacher: **0.9366 mIoU**
  - Student Phase-1: **0.9115 mIoU** (best at epoch 10, 23 epochs total)
  - Student Phase-2: **0.9364 mIoU** (best at epoch 12, 15 epochs total)
- **Efficiency**: linear FLOPs reduced by **~5×**, while maintaining **teacher-level accuracy**.

---

## 📊 Training Curves

<p align="center">
  <img src="phase1_curve.png" alt="Phase-1 curve" width="45%"/>
  <img src="phase2_curve.png" alt="Phase-2 curve" width="45%"/>
</p>

---

## 🔁 Reproducibility

To reproduce results, simply open the Jupyter Notebook:

    jupyter notebook article0_run.ipynb

The notebook contains all logs and code to regenerate training curves.  
Checkpoints for Phase-1 and Phase-2 are available on the Google Drive link above.

---

## 📜 Citation

If you find this work useful, please cite:

    @article{druzhinin2025lora_la,
      title={Efficient Student Segmentation: Reducing Linear Layer Computations with Near-Teacher Accuracy},
      author={Aleksandr Druzhinin},
      journal={arXiv preprint arXiv:XXXX.XXXXX},
      year={2025}
    }

---

## 📄 License
This project is licensed under the MIT License — see the LICENSE file for details.

---

## 📧 Contact
For questions, please contact: sdruzhinin1992@gmail.com
