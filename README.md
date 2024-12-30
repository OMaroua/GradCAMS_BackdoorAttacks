# GradCAMS_BackdoorAttacks
In this project,I focus on poisoning-based backdoor attacks, where the training dataset is manipulated to implant triggers. Through this, I investigate the behavior of backdoored models, analyze their susceptibility to triggers, and evaluate Grad-CAM visualizations to understand how the model’s decision-making process is affected.


Contents of the Project:
1. **Clean_Model**: Contains the trained clean ResNet50 model.

2. **Backdoor_attack1**: Implements a basic backdoor attack with red stripe trigger.
   - `basic_attack.ipynb`: Jupyter notebook for the backdoor attack.

3. **Backdoor_attack_triangle**: Implements a triangle-based backdoor attack.
   - `Triangle_attack.ipynb`: Jupyter notebook for the triangular pattern backdoor attack.


For more information, refer to the documentation in `USAGE.txt`.
