# Awomo-Video: Learning Physical Dynamics from Structured Captions and Robot Actions

[Project Page](https://westlakedi-awomo.github.io/Awomo-WM-Page/) · [Technical Report](https://github.com/westlake-autolab/Awomo-WM-Technical-Report)

> **Release status:** This repository is a placeholder for the forthcoming Awomo-Video code release. Inference and training code are not yet available.

## Overview

Awomo-Video is a video world model designed to generate visually coherent sequences that better reflect how objects move, interact, and change state. It combines physically grounded data curation and structured supervision with two complementary generation settings:

- **Text-image-to-video (TI2V):** generates a future video from a reference image and a textual description while preserving the observed scene and modeling its subsequent dynamics.
- **Image-action-to-video (IA2V):** generates robot-view video from a reference image and a sequence of robot actions, connecting commanded motion with the evolution of the visual scene.

The method is developed around a physical data pipeline that retains observable interactions, filters technical and semantic artifacts, and organizes supervision into structured descriptions of scenes, entities, camera behavior, material properties, and temporally localized events. Awomo-Video-TI2V combines multimodal reference conditioning with first-frame-constrained flow matching. Awomo-Video-IA2V incorporates end-effector action trajectories and supports both bidirectional training and causal rollout generation.

## Highlights

- **Physically grounded supervision.** Structured captions distinguish object behavior from camera motion and describe entities, materials, spatial relationships, and temporal dynamics.
- **Balanced video training.** Dynamic sampling combines general-domain and physics-focused video pools to strengthen physical modeling while retaining broad generation capabilities.
- **Two complementary generation interfaces.** TI2V supports image-and-language-conditioned generation, while IA2V models robot observations conditioned on action trajectories.
- **Strong physical-video performance.** Awomo-Video achieves a 45.5% Physics-IQ Verified Score in the evaluation reported in the technical report.
- **Embodied-world modeling.** The IA2V formulation connects end-effector commands with visual predictions of robot interaction sequences.

## TODO

- [ ] Release Awomo-Video-TI2V inference code.
- [ ] Release Awomo-Video-TI2V training code.
- [ ] Release Awomo-Video-IA2V inference code.
- [ ] Release Awomo-Video-IA2V training code.

Please stay tuned for future updates.
