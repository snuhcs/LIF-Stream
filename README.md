# LIF-Stream

Official code for **Spiking Neural Networks Incrementally Track Firing-Rate Networks**
by Hyunseok Oh and Youngki Lee (Seoul National University).

[[Paper (arXiv)]](https://arxiv.org/abs/XXXX.XXXXX)

> **Code coming soon.** The code will be released in this repository. Watch or star the repository to get notified.

## Overview

We prove that the output of a discrete spiking neural network (SNN) with leaky integrate-and-fire (LIF) neurons continuously tracks the instantaneous output of its corresponding firing-rate network (a continuous-valued ReLU1 network), implicitly determined by the SNN input.

Based on this principle, **LIF-Stream** is an ANN-to-SNN conversion framework for efficient SNN inference over unbounded data streams:

- **Incremental computation.** The converted SNN keeps its state across frames and computes only the activation updates between frames, so it needs fewer time steps per frame on average.
- **No global reset.** Standard LIF neurons with soft reset, converted from an ordinary frame-wise ReLU1 network. No specialized training, fine-tuning, or custom neuron dynamics.
- **High accuracy on every frame.** The SNN continuously tracks the reference ANN output.

LIF-Stream is evaluated on three large-scale streaming benchmarks with distinct modalities: streaming object detection, streaming speech recognition, and event-stream gesture recognition.

## Citation

```bibtex
@article{oh2026lifstream,
  title   = {Spiking Neural Networks Incrementally Track Firing-Rate Networks},
  author  = {Oh, Hyunseok and Lee, Youngki},
  journal = {arXiv preprint arXiv:XXXX.XXXXX},
  year    = {2026}
}
```

## Contact

Hyunseok Oh (ohsai@snu.ac.kr)
