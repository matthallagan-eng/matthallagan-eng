# Matthew Hallagan

Controls engineer building software for manufacturing.

I work at the intersection of industrial automation, manufacturing systems, and computer vision—where plant floor problems become software problems.

Over the past four years, I’ve worked in food and pharmaceutical manufacturing with PLCs, SCADA, MES, industrial networks, SQL databases, and Ignition. Along the way, I found that the most interesting challenges are often not in the control system itself, but in turning manufacturing data into information people can actually use.

Manufacturing generates enormous amounts of data, but much of the most valuable information never enters a database at all. It exists on labels, gauges, displays, operator panels, and products moving down a line. Cameras are inexpensive, computer vision models are powerful, and edge hardware is widely available—but building systems that are reliable enough for production is still difficult.

That gap between a proof of concept and a tool operators can trust is the problem I keep coming back to.

---

## Projects

### FloorSight

**Production monitoring and OEE analytics**

A web application for analyzing production performance using uploaded datasets or live simulations.

Live Demo: https://floorsight-gamma.vercel.app/
* Username: demo@floorsight.app
* Password: demotest

Features:

* OEE breakdown into Availability, Performance, and Quality
* Downtime Pareto analysis to identify major losses
* Interactive dashboards and production metrics
* FastAPI backend with PostgreSQL
* React + TypeScript frontend
* Dockerized deployment on Railway and Vercel

**Tech:** FastAPI · PostgreSQL · React · TypeScript · Docker

---

### LabelLint *(In Progress)*

**Dataset quality tools for computer vision**

A toolkit for finding annotation issues before training models.

Checks include:

* Duplicate images
* Degenerate or invalid bounding boxes
* Class imbalance detection
* Dataset statistics and validation
* Conversion between YOLO, COCO, and Pascal VOC formats

This project came from repeatedly seeing the same pattern: in many computer vision projects, the dataset is the bottleneck—not the model.

**Tech:** Python · OpenCV · PyTorch

---

## Professional Background

Currently a Corporate Controls Engineer supporting four US manufacturing plants and leading a company-wide migration from legacy MES and shopfloor systems to Ignition.

---

## Computer Vision Work

Built proof-of-concept systems using YOLO, OpenCV, PyTorch, and Roboflow, including:

* Gauge readers
* Digital display OCR
* Stack light monitoring
* Tool and component detection
* Vision systems publishing results into Ignition over MQTT

Most of the work has been in the less glamorous but more important parts of vision systems:

* Dataset collection
* Annotation quality
* Reducing false positives
* Edge deployment
* Integrating models into existing industrial systems

---

## Technologies

**Industrial:** PLCs · Ignition · SCADA · MES · MQTT · Industrial Networks

**Software:** Python · TypeScript · FastAPI · React · PostgreSQL · Docker

**Computer Vision:** YOLO · OpenCV · PyTorch · Roboflow

