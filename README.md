@article{zhang2023diffusionad,
  title={DiffusionAD: Norm-guided One-step Denoising Diffusion for Anomaly Detection},
  author={Zhang, Hui and Wang, Zheng and Wu, Zuxuan and Jiang, Yu-Gang},
  journal={arXiv preprint arXiv:2303.08730},
  year={2023}
}

MVTec-AD
|-- carpet
|-----|----- thresh
|-----|----- ground_truth
|-----|----- test
|-----|--------|------ good
|-----|--------|------ ...
|-----|----- train
|-----|--------|------ good
|-- cable
|-----|----- DISthresh
|-----|----- ground_truth
|-----|----- test
|-----|--------|------ good
|-----|--------|------ ...
|-----|----- train
|-----|--------|------ good

VisA
|-- candle
|-----|----- DISthresh
|-----|----- ground_truth
|-----|----- test
|-----|--------|------ good
|-----|--------|------ bad
|-----|----- train
|-----|--------|------ good
|-- capsules
|-- ...

Environment
pip install -r requirements.txt

Train
Please specify the dataset path(MVTec-AD,VisA), anomaly_source_path(DTD), and output folder in args.json and run:
python train.py

Evaluation
python eval.py
