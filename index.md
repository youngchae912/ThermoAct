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
<div class="content has-text-justified" style="margin-top: 10px;">
  <p>
  The ThermoAct framework proposed in this study consists of a Vision-Language Model (VLM) that performs reasoning and planning based on user commands and environmental information, and a Vision-Language-Action (VLA) module that executes robot control commands based on this plan. The VLM takes visual inputs, including thermal data, and a natural language instruction to generate a low-level action plan tailored to the situation. Subsequently, the VLA module controls the robot in real-time based on the decomposed plan and the corresponding inputs.
  </p>
</div>

<section class="hero teaser" style="padding: 0;">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <video id="teaser1" autoplay muted loop playsinline height="100%">
        <source src="static/image/thermoact_video.mp4" type="video/mp4">
      </video>
    </div>
  </div>
</section>

<div class="container is-max-desktop">
  <div class="columns is-vcentered">
    <div class="column is-half">
      <div class="content has-text-justified">
        <p>
          All tasks were designed to require the successful completion of not only temperature-aware sub-tasks but also everyday sub-tasks (e.g., clearing unused cables, placing an apple on a plate). The sub-tasks decomposed by the VLM Planner follow a standardized format, aligning with protocols used in recent VLM-based robotic planning.
        </p>
        <p>
          Task 1 to Task 3 were designed to evaluate whether the robot could act more intelligently by utilizing thermal information in daily scenarios, such as handing over a cup of warm water or giving a cold can of soda. 
        </p>
        <p>
          Task 4 and Task 5 was designed to verify the utility of thermal information in safety-related situations, such as picking up an overheated battery, turning off a hot hair straightener, and organizing the nearby power strip.
        </p>
      </div>
    </div>
    <div class="column is-half">
      <figure class="image">
        <img src="static/image/Fig3.png" alt="Experimental Results and Task Visualization">
        <p class="has-text-centered is-size-7 mt-2">
          <strong>Figure 3:</strong> Task design and VLM planning protocol.
        </p>
      </figure>
    </div>
  </div>
</div>

<hr>
<h2 class="title is-3 has-text-centered mt-6 mb-5">Experiment in Real-World</h2>

<div class="box" style="background-color: #f5f5f5; border: 1px solid #e8e8e8; margin-bottom: 2rem;">
  <div class="columns is-centered">
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 2: Give me a cold coke (w/ cold coke)</h3>
        <video id="video1" controls loop playsinline width="100%">
          <source src="static/image/task2.mp4" type="video/mp4">
        </video>
      </div>
    </div>
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 2: Give me a cold coke (w/o cold coke)</h3>
        <video id="video2" controls loop playsinline width="100%">
          <source src="static/image/task2_2.mp4" type="video/mp4">
        </video>
      </div>
    </div>
  </div>
</div>

<div class="box" style="background-color: #f5f5f5; border: 1px solid #e8e8e8; margin-bottom: 2rem;">
  <div class="columns is-centered">
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 3: Select the appropriate cup (teabag)</h3>
        <video id="video3" controls loop playsinline width="100%">
          <source src="static/image/task3.mp4" type="video/mp4">
        </video>
      </div>
    </div>
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 3: Select the appropriate cup (lemon)</h3>
        <video id="video4" controls loop playsinline width="100%">
          <source src="static/image/task3_2.mp4" type="video/mp4">
        </video>
      </div>
    </div>
  </div>
</div>

<div class="box" style="background-color: #f5f5f5; border: 1px solid #e8e8e8; margin-bottom: 2rem;">
  <div class="columns is-centered">
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 4: Pick up overheated battery</h3>
        <video id="video5" controls loop playsinline width="100%">
          <source src="static/image/task4.mp4" type="video/mp4">
        </video>
      </div>
    </div>
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 4: Pick up overheated battery</h3>
        <video id="video6" controls loop playsinline width="100%">
          <source src="static/image/task4_2.mp4" type="video/mp4">
        </video>
      </div>
    </div>
  </div>
</div>

<div class="box" style="background-color: #f5f5f5; border: 1px solid #e8e8e8; margin-bottom: 2rem;">
  <div class="columns is-centered">
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 5: Organize space near power strip</h3>
        <video id="video7" controls loop playsinline width="100%">
          <source src="static/image/task5.mp4" type="video/mp4">
        </video>
      </div>
    </div>
    <div class="column">
      <div class="content">
        <h3 class="title is-5 has-text-centered">Task 5: Organize space near power strip</h3>
        <video id="video8" controls loop playsinline width="100%">
          <source src="static/image/task5_2.mp4" type="video/mp4">
        </video>
      </div>
    </div>
  </div>
</div>
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
