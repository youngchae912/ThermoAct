---
layout: project_page
permalink: /

title: "ThermoAct: Thermal-Aware Vision-Language-Action Models \\for Robotic Perception and Decision-Making"
authors:
  - Young-Chae Son, Dae Kwan Ko, Yoon Ji Choi and Soo-Chul Lim*
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
In recent human-robot collaboration environments, there is a growing focus on integrating diverse sensor data beyond visual information to enable safer and more intelligent task execution. Although thermal data can be crucial for enhancing robot safety and operational efficiency, its integration has been relatively overlooked in prior research. This paper proposes a novel Vision-Language-Action (VLA) framework that incorporates thermal information for robot task execution. The proposed system leverages a Vision-Language Model (VLM) as a high-level planner to interpret complex natural language commands and decompose them into simpler sub-tasks. This approach facilitates efficient data collection and robust reasoning for complex operations. Unlike conventional methods that rely solely on visual data, our approach integrates thermal information, enabling the robot to perceive physical properties and proactively ensure environmental safety. Experimental results from real-world task scenarios validate the feasibility of our proposed framework, suggesting its potential to enhance task success rates and safety compared to existing vision-based systems.
        </div>
    </div>
</div>

---
## Framework
![Framework](/static/image/Fig1.png)

<section class="hero teaser" style="padding: 0;">
  <div class="container is-max-desktop" style="padding: 0;">
    <div class="hero-body" style="padding: 0; position: relative;">
      <video 
        id="teaser1" 
        autoplay 
        muted 
        loop 
        playsinline 
        style="width: 100%; height: auto; display: block; object-fit: cover;">
        <source src="/static/image/thermoact_video1.mp4" type="video/mp4">
      </video>
      <div class="content has-text-justified" style="margin-top: 10px;">
        <p>
        The ThermoAct framework proposed in this study consists of a Vision-Language Model (VLM) that performs reasoning and planning based on user commands and environmental information, and a Vision-Language-Action (VLA) module that executes robot control commands based on this plan. The VLM takes visual inputs, including thermal data, and a natural language instruction to generate a low-level action plan tailored to the situation. Subsequently, the VLA module controls the robot in real-time based on the decomposed plan and the corresponding inputs.
        </p>
      </div>

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
        <source src="static/image/thermoact_video2.mp4" type="video/mp4">
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
