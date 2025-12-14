<!-- SYNC IMPACT REPORT
Version change: 0.1.0 → 1.0.0
Modified principles: All principles updated from template values
Added sections: Key Standards, Constraints and Technical Requirements
Removed sections: None
Templates requiring updates: 
- ✅ .specify/templates/plan-template.md
- ✅ .specify/templates/spec-template.md  
- ✅ .specify/templates/tasks-template.md
- ⚠ .specify/templates/commands/*.md - needs review
- ⚠ README.md - needs review
Follow-up TODOs: None
-->

# Physical AI & Humanoid Robotics Textbook Constitution

## Core Principles

### Technical Accuracy
All content must strictly align with official documentation: ROS 2 Humble, Gazebo/Ignition, Unity Robotics Hub, NVIDIA Isaac Sim 4.x, OpenAI API & VLA developer docs. This ensures that all instructions, code, and explanations match the actual behavior of the systems being taught.

### Learnability
Content must be structured, beginner-friendly, and suitable for CS/AI/Robotics students. All concepts should be introduced with clear explanations before moving to implementation details, ensuring students can follow along regardless of their prior experience level.

### Hands-On Orientation
Every concept must include runnable simulations, working code, reproducible experiment steps. Theory without practice is ineffective for robotics education; all content must include hands-on activities that students can perform to reinforce learning.

### Safety First
All robotics instructions must follow standard hardware & simulation safety. This includes proper setup procedures, safe operation guidelines, and risk mitigation strategies for both physical and simulated environments.

### Modularity
Each chapter must stand alone and be navigable independently. Students should be able to pick and choose modules relevant to their needs without having to work through prerequisite chapters in sequence.

### Accessibility
Textbook must build cleanly in Docusaurus and deploy perfectly on GitHub Pages. This ensures that the content is accessible to all students regardless of their computing environment or physical abilities.

## Key Standards

### Code Quality
All code must be tested & runnable. Include environment setup and troubleshooting. Python, ROS 2, URDF/XACRO must follow best practices. This ensures that students can reproduce all examples without running into technical issues.

### Documentation Sources
Only use verifiable official sources. All information must be traceable to official documentation from ROS 2, Gazebo, Unity, NVIDIA Isaac, or OpenAI to ensure accuracy and maintainability.

### Images & Simulations
Screenshots and diagrams must match real simulation output. Visual aids must accurately represent the actual output that students will see when following instructions, preventing confusion and frustration.

### Writing Standards
Professional engineering tone, Step-by-step instructions, No filler content, only actionable material. Content should be clear, concise, and focused on helping students achieve specific learning objectives.

## Constraints and Technical Requirements

### Book Format
Docusaurus v3, GitHub Pages deployment, Markdown-based chapters. The technical constraints ensure consistent deployment and maintainability across the project lifecycle.

### Chapter Requirements
Each chapter (10–20 pages) must include learning objectives, code samples, diagrams, simulation walkthrough, troubleshooting. These requirements ensure consistent quality and coverage across all textbook modules.

### Technical Requirements
Ubuntu 22.04, ROS 2 Humble, Python 3.12+, Hardware focus: low-cost educational robots or simulation-only. These platform constraints ensure that content is accessible to students with limited resources while maintaining compatibility with current industry tools.

## Success Criteria

* All instructions error-free
* All simulations run exactly as documented
* `npm run build` passes
* GitHub Pages deploys with no broken links
* RAG chatbot answers correctly using textbook content
* Peer review passes
* Code executes correctly
* Navigation clear & modular
* Diagrams match simulation results

## Spec-Kit Plus Workflow (Mandatory)

Each module must follow the Spec-Kit Plus pipeline:

1. **/sp.constitution** → Project constitution (this file)
2. **/sp.specify** → Chapter-level specifications
3. **/sp.clarify** → Requirement refinement
4. **/sp.plan** → Full implementation plan
5. **/sp.tasks** → Break into atomic tasks
6. **/sp.implement** → Generate content and code
7. **/sp.adr** → Architectural decisions

No manual file creation.

## Module Coverage (Mandatory)

### Module 1: ROS 2 Foundations
* Nodes, topics, services
* URDF/XACRO robot modeling
* RViz visualization
* Basic mobile robot simulation

### Module 2: Gazebo/Unity Simulation
* World building
* Physics engines
* Sensors: Camera, LiDAR, IMU
* Exporting ROS 2–compatible environments

### Module 3: NVIDIA Isaac (Perception + RL)
* Camera streaming
* Object detection
* Synthetic data generation
* RL with Isaac Lab

### Module 4: VLA (Vision‑Language‑Action)
* GPT + Whisper
* Perception→Action pipelines
* Language‑based robot control
* Multi-step reasoning

## Core Deliverables

* Complete Docusaurus textbook
* GitHub repo with:
  * markdown chapters
  * images
  * simulation files
  * ROS 2 packages
* Fully deployable GitHub Pages site
* RAG chatbot powered by the textbook
* Full Spec-Kit Plus project with specs, tasks, ADRs, PHRs

## Governance

All textbook content must follow the Spec-Kit Plus workflow ensuring systematic development and documentation. All modules must cover the required curriculum areas. Changes to this constitution require explicit approval and documentation via the Spec-Kit Plus process.

**Version**: 1.0.0 | **Ratified**: 2025-12-09 | **Last Amended**: 2025-12-09