---
layout: project_page
permalink: /

title: "MulPhyLM: Multimodal Robotic Planning through Vision-Language Models and Physical Interaction"
authors:
  - Young-Chae Son, DongHan Lee and Soo-Chul Lim*
affiliations:
  - Dongguk University, Seoul 04620, South Korea
paper: https://www.cs.virginia.edu/~robins/Turing_Paper_1936.pdf
video: https://www.youtube.com/results?search_query=turing+machine
code: https://github.com/topics/turing-machines
data: https://huggingface.co/docs/datasets
---

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
This study proposes a robot task automation framework based on large language models (LLMs) that utilizes both visual and physical information. The system integrates multimodal inputs, including camera images and force/torque (F/T) sensor data, to interpret the visual and physical state of objects and generate a task sequence to execute given commands. The integration of vision and force data allows the system to compensate for the limitations of each modality, leading to more reliable decision-making. The framework consists of three components: Extractor, Planner, and Sub-planner. According to their assigned roles, each agent automatically translates high-level commands given in natural language into executable robot motion plans, enabling the robot to perform the required sequence of actions. The system combines visual and force data to handle tasks that are difficult or infeasible with a single modality. Furthermore, it supports sequential and condition-based task planning through the collaboration of multiple LLM agents. Experimental results in various task scenarios show that the proposed framework operates reliably with different LLMs and achieves a higher success rate compared to using only visual or force data.
        </div>
    </div>
</div>

---
## Framework
![Framework](/static/image/figure1.png)

<section class="hero teaser" style="padding: 0;">
  <div class="container is-max-desktop" style="padding: 0;">
    <div class="hero-body" style="padding: 0; position: relative;">
      <video 
        id="teaser" 
        autoplay 
        muted 
        loop 
        playsinline 
        style="width: 100%; height: auto; display: block; object-fit: cover;">
        <source src="static/image/testvideo.mp4" type="video/mp4">
      </video>
    </div>
  </div>
</section>

<section class="hero teaser" style="padding: 0;">
  <div class="container is-max-desktop" style="padding: 0;">
    <div class="hero-body" style="padding: 0; position: relative;">
      <video 
        id="teaser" 
        autoplay 
        muted 
        loop 
        playsinline 
        style="width: 100%; height: auto; display: block; object-fit: cover;">
        <source src="static/image/testvideo2.mp4" type="video/mp4">
      </video>
    </div>
  </div>
</section>


## Citation
```
@article{turing1936computable,
  title={On computable numbers, with an application to the Entscheidungsproblem},
  author={Turing, Alan Mathison},
  journal={Journal of Mathematics},
  volume={58},
  number={345-363},
  pages={5},
  year={1936}
}
```
