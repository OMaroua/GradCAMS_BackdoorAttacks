USAGE

This project implements and visualizes Grad-CAM for analyzing clean models and models compromised with backdoor attacks, including a triangular dot pattern and a red stripe trigger. Below are instructions to run the provided Jupyter notebooks and Python scripts for each scenario.

---

### 1. Prerequisites

- Ensure you have access to a GPU for faster training and evaluation (optional but recommended).

---

### 2. Code Scenarios
This project includes three primary implementations:
1. **Clean Model:**
   - Fine-tunes a ResNet50 model on the Oxford-IIIT Pet Dataset.
   - Evaluates the clean model with Grad-CAM visualizations.

2. **Red Stripe Backdoor Attack:**
   - Injects a red stripe as a backdoor trigger.
   - Retrains the ResNet50 model on the poisoned dataset.
   - Evaluates the backdoored model with Grad-CAM visualizations.

3. **Triangle Backdoor Attack:**
   - Injects a triangular dot pattern as a backdoor trigger.
   - Retrains the ResNet50 model on the poisoned dataset.
   - Evaluates the backdoored model with Grad-CAM visualizations.

---

### 3. Running the Notebooks
- **For Clean Model:**
  - Retrain the model using the notebook/script or load the pre-trained model (`resnet50_oxfordiiitpet_full.pth`).
  - Evaluate the clean model using Grad-CAM on the test dataset.

- **For Triangle Backdoor Attack:**
  - Inject the triangular dot pattern trigger into the dataset.
  - Retrain the model or load the pre-trained backdoored model (`resnet50_backdooredtriangle.pth`).
  - Evaluate the backdoored model and visualize Grad-CAM to analyze its focus.

- **For Red Stripe Backdoor Attack:**
  - Inject the red stripe trigger into the dataset.
  - Retrain the model or load the pre-trained backdoored model (`resnet50_backdoored10.pth`).
  - Evaluate the backdoored model and analyze Grad-CAM visualizations.

---

### 5. Grad-CAM Visualizations
1. Load a test image from the clean or poisoned test dataset.
2. Use Grad-CAM to highlight the regions influencing the model's predictions:
   - **Original Image:** Displays the input image.
   - **Grad-CAM Heatmap:** Highlights the areas the model focused on.
   - **Overlay Image:** Combines the heatmap with the original image for interpretability.

3. Example Outputs:
   - Clean Model: Grad-CAM focuses on meaningful features like the pet's face or body.
   - Backdoored Models: Grad-CAM highlights backdoor trigger regions (triangle dots or red stripe) instead of legitimate features.

---

### 6. Outputs
- **Model Weights:**
  - Clean Model: `resnet50_oxfordiiitpet_full.pth`
  - Triangle Backdoored Model: `resnet50_backdooredtriangle.pth`
  - Red Stripe Backdoored Model: `resnet50_backdoored10.pth`

- **Visualizations:**
  - Displayed inline in the notebooks.
  - Can be manually saved by right-clicking on the plots.
