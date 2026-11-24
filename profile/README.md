<p align="center">
  <a href="https://roboada.github.io"><img src="https://raw.githubusercontent.com/RoboAda/RoboAda/main/docs/figures/teaser.svg" width="100%" alt="RoboAda overview"></a>
</p>

<h2 align="center">RoboAda: Adapting Frozen Robot Policies at Test Time to Physics They Cannot See</h2>

<p align="center">
  Yunbei Zhang<sup>1</sup> &nbsp; Zijian Jin<sup>2</sup> &nbsp; Shuaicheng Niu<sup>3</sup> &nbsp; Baian Chen<sup>4</sup> &nbsp; Weirui Ye<sup>4</sup> &nbsp; Jihun Hamm<sup>1</sup> &nbsp; Yilun Du<sup>5</sup><br>
  <sup>1</sup>Tulane &nbsp; <sup>2</sup>NYU &nbsp; <sup>3</sup>NTU &nbsp; <sup>4</sup>MIT &nbsp; <sup>5</sup>Harvard
</p>

<p align="center">
  <a href="https://roboada.github.io"><b>Project page</b></a> &nbsp;|&nbsp; <a href="https://github.com/RoboAda/RoboAda"><b>Code</b></a> &nbsp;|&nbsp; <a href="https://roboada.github.io/assets/RoboAda.pdf"><b>Paper</b></a>
</p>

A heavier object, a weakened joint or a lagging controller looks the same in a camera image, yet it changes how a robot
moves. RoboAda keeps a pretrained policy frozen and corrects its commands by inferring, after every action chunk, how the
robot now turns commands into motion. It needs no reward, no gradient step and no data from the changed robot, and it
wraps world action models and vision-language-action models alike.

| Repository | What is in it |
|---|---|
| [RoboAda](https://github.com/RoboAda/RoboAda) | The method in numpy, a quickstart that runs in seconds without a simulator, an API for your own policy (Python function, HTTP endpoint or openpi server) and the LIBERO evaluation |
| [RoboAda.github.io](https://github.com/RoboAda/RoboAda.github.io) | The project page, with an interactive demo and an animation of the method |

```bash
git clone https://github.com/RoboAda/RoboAda.git
cd RoboAda && pip install -e . && python examples/quickstart.py
```
