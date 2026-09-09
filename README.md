Matthew Hallagan

Controls and systems engineer. Four years in food and pharmaceutical manufacturing working with PLCs, SCADA, MES, and industrial networks, and building software around the same problems.

Most of what I work on sits where the plant floor meets the software layer. Manufacturing generates enormous amounts of data and very little of it ends up somewhere people can act on. That gap is what I find interesting.

Lately that has pulled me toward computer vision. A lot of what plants need to know is visible on the floor and nowhere else: whether a label printed correctly, what a gauge reads, whether a part came out right. Cameras are cheap and models are good now, but getting from a working proof of concept to something a plant can actually rely on is still the hard part. That is the problem I keep coming back to.

Projects

FloorSight — Production monitoring and OEE analytics Upload production data or run a live simulation. Breaks OEE into availability, performance, and quality, with downtime sorted into a Pareto so you can see what to fix first. FastAPI, PostgreSQL, React, TypeScript, Docker, deployed on Railway and Vercel. Live demo

LabelLint — Dataset quality checks for computer vision (in progress) Finds the problems in an annotation set before you spend a GPU day on it. Duplicates, degenerate boxes, class imbalance, and format conversion between YOLO, COCO, and Pascal VOC. Came out of noticing that on every CV project I worked on, the dataset was the bottleneck rather than the model.

Background

Currently a corporate controls engineer supporting four US manufacturing plants, leading an MES and shopfloor migration to Ignition across all four sites. Previously automation controls at Perrigo's infant formula division, where I led a $1.5M dryer control system upgrade and built a SQL-based recipe management system bridging SAP and PLC setpoints.

On the vision side I have built detection and OCR proofs of concept with YOLO, OpenCV, PyTorch, and Roboflow, including an instrumentation reader that pulls values off gauges, digital displays, and stack lights and publishes them into Ignition over MQTT. Most of my time there has gone into the unglamorous parts: dataset collection and labeling, chasing false positives, and working out where edge deployment makes more sense than cloud.

Python · TypeScript · FastAPI · React · PostgreSQL · Docker · PyTorch · OpenCV · YOLO · Ignition · MQTT · PLC
