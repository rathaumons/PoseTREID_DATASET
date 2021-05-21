# PoseTReID and Dataset

### What is PoseTReID?

![alt text](https://raw.githubusercontent.com/rathaumons/PoseTReID_DATASET/master/img/framework.png)

We propose a framework for real-time 2D multi-person tracking along with face re-identification specifically for distributed people interaction spaces such as malls or parks. Our proposed framework is able to efficiently track people and re-identify them later after the tracking is lost or after the absence of the people at some frames of the video.

More details? COMING SOON!

### Dataset

![alt text](https://raw.githubusercontent.com/rathaumons/PoseTReID_DATASET/master/img/dataset_overview.jpg)

All videos were rendered in 16:9 ratio at a resolution of 1080p with our custom script. Afterwards, they were down-scaled to 720p to fit our real-time testing scenarios and more realistic real-life cameras with less good resolution. 

This dataset is specifically designed for **either indoor like in malls, outdoor like in smart cities, or in both situations like in amusement parks, where faces are visible enough to be recognized**.

The ground truth is provided in 2 different formats such as `.txt` and `.csv` for every video with two choices of ID such as number or real name.

### Results
By comparing to a state-of-the-art recent method [STAF](https://cmu-perceptual-computing-lab.github.io/spatio-temporal-affinity-fields/) on our dataset, the results of the proposed PoseTReID model were superior in almost every scenarios.

For **real-time video comparison**: [CLICK HERE!](https://drive.google.com/open?id=1WLGrRAdQPV-tA9B2OZPEwwMvFDVAymqX)

| Complexity | Camera Conf. | STAF | Tracking only | Full mode |
| :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
| Normal | Low | 85.28% | 85.35% | 97.13% |
| Normal | High | 85.05% | 100% | 96.85% |
| Hard | Low | 41.13% | 38.36% | 91.31% |
| Hard | Front | 38.39% | 38.36% | 89.00% |
| Hard | High | 59.70% | 56.02% | 89.93% |
| Hard | Surveillance | 86.22% | 85.96% | 40.71% |

### Citation
Please kindly cite this paper if you find it helpful for your research.
```
@INPROCEEDINGS{ptreid9271712,
  author={Siv, Ratha and Mancas, Matei and Sreng, Sokchenda and Chhun, Sophea and Gosselin, Bernard},
  booktitle={2020 12th International Conference on Information Technology and Electrical Engineering (ICITEE)}, 
  title={People Tracking and Re-Identifying in Distributed Contexts: PoseTReID Framework and Dataset}, 
  year={2020},
  pages={323-328},
  doi={10.1109/ICITEE49829.2020.9271712}}
```
