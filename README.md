# DCTracker
DCTracker: Rethinking MOT in Soccer Events Under Dual Views via Cascade Association.

Long Hu, Junjie Zhang, Weiyi Lv, Yongshun Gong, Jingya Wang, Jian Zhang and Dan Zeng

It is currently accepted in the journal Knowledge-Based Systems (2024/09). DOI：https://doi.org/10.1016/j.knosys.2024.112528.

# Abstract
Multi-Object Tracking (MOT) presents promising applications in intelligent sporting event analysis. Existing models primarily cater to pedestrian-dominant scenarios with fixed camera locations and linear motion trajectories. However, sporting events introduce unique challenges: (i) cameras exhibit significant movement and dynamic focal length changes, causing drastic shifts in player positions between frames. (ii) player motion trajectories are nonlinear and influenced by game trends, resulting in complex, fast-paced behaviors compounded by irregular camera motions. (iii) challenges such as image blurring, occlusion, and similar player appearances complicate the maintenance of robust and distinctive identification-related visual states. 
These challenges pose significant barriers for the application of off-the-shelf trackers. To address above issues, we introduce DCTracker, a novel multi-object tracker tailored for robust performance in soccer games. The approach corrects the state estimation of the conventional Kalman filter by integrating homography for the bird's-eye-view perspective and inter-frame registration for broadcast view, known as the dual-view Kalman filter (DVKF). DVKF extends the estimation model to obtain multi-state vectors for objects, mitigating the impact of camera motion and non-linear player trajectories. Additionally, a cascade selection module (CSM) is proposed, leveraging spatial topological relationships between players to address blurry and occluded visual appearances. The resulting cost matrices are adaptively employed to establish correct associations, significantly reducing identity switches. The proposed method achieves state-of-the-art performances on the test set of SoccerNet-Tracking and the validation split of SportsMOT-soccer. Experimental results demonstrate that the proposed approach performs satisfactorily in soccer events characterized by a wide range of venues and non-linear player trajectories.


# Tracking performance
| Datasets           | HOTA ↑ | MOTA ↑ | IDF1 ↑ | FN ↓ | FP ↓ | IDSW ↓ | Frag ↓ | DetA ↑ | AssA ↑ |
|-------------------|--------|--------|--------|-------|-------|--------|--------|--------|--------|
| SoccerNet-Tracking test  | 67.0 | 88.8 | 77.4 | 44259 | 17281 | 1801 | 7063   | 73.9 | 60.8 |
| SportsMOT-Soccer val | 74.6 | 93.0 | 76.2 | 2417 | 5469 | 331 | 538 | 84.4 | 65.9 |

# Installation

The code will be uploaded soon.
