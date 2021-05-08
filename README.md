# AgeVoxCeleb

## AgeVoxCeleb DATABASE
The AgeVoxCeleb is the large-scale, balanced,
and multi-modal age corpus that contains both video and speech of the same speakers
from a wide age range. 

The AgeVoxCeleb contains nearly 168k videos of approximately 5000 speakers selected 
from [VoxCeleb2](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox2.html).
All the videos are labeled with the speaker’s real age estimated 
using each celebrity's name and title of the original YouTube video.
 
To know the detail of how we built AgeVoxceleb, please refer to our paper 
presented in [ICASSP2021](https://ieeexplore.ieee.org/document/9414272/).

### USAGE
In this repository, only annotation labels are distributed.
To obtain the data including audio files, cropped video files, and other meta information,
please visit the original web-page of [VoxCeleb2](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox2.html) and download them.

### Data description

Each line in ``utt2spk.train`` and ``utt2spk.test`` corresponds to a pair of the segment-id and annotated age labels 
in training and test sets. 
Note that the segment-id is composed of speaker-ID, video-ID, and segment-ID defined in the original VoxCeleb. 

In addition, please note that how to divide the data into training and test sets is different from ones defined in the original VoxCeleb dataset.

### Citation
If you use this dataset, please cite:
```
@inproceedings{tawara2021age,
  title={Age-VOX-Celeb: Multi-Modal Corpus for Facial and Speech Estimation},
  author={Tawara, Naohiro and Ogawa, Atsunori and Kitagishi, Yuki and Kamiyama, Hosana},
  booktitle={ICASSP 2021-2021 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={6963--6967},
  year={2021},
  organization={IEEE}
}
```