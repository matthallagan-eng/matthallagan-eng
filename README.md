# Matthew Hallagan

Engineer at [Overview AI](https://www.overview.ai), building AI vision systems for manufacturing.

I work where industrial automation, manufacturing systems, and computer vision meet: the place where plant floor problems turn into software problems.

I spent four years in food and pharmaceutical manufacturing working with PLCs, SCADA, MES, industrial networks, SQL databases, and Ignition. The most interesting problems were rarely inside the control system. They were about turning manufacturing data into information people could actually use.

Much of the most valuable information on a plant floor never reaches a database. It lives on labels, gauges, displays, operator panels, and the products moving down the line. Cameras are cheap, vision models are powerful, and edge hardware is everywhere, but building systems reliable enough for production is still hard.

The gap between a proof of concept and a tool operators can trust is the problem I keep coming back to, and it's the problem I now work on full time at Overview AI.

---

## Current Project

### DiveDebrief

**A dive log that coaches you**

Live Demo: https://divedebrief.up.railway.app/
* Username: demo@divedebrief.app
* Password: divedemo2026

Repo: https://github.com/matthallagan-eng/divedebrief

Upload the files from your dive computer and DiveDebrief scores how well each dive went, explains every score in plain words, and gives you one thing to work on next time.

* Imports Garmin FIT and UDDF logs (Subsurface exports), deduplicated by start time
* Scores ascent control, safety stop, buoyancy, and air efficiency from 0 to 100, each with its reason and a link to the moment on the profile that cost points
* Shows N/A with an explanation when a skill can't be scored, instead of a made-up number
* Rule-based debrief with a goal for your next dive, then checks how you did against it. No AI, so the advice is predictable and testable
* Depth profiles with ascent-rate violations highlighted, plus optional graphs for heart rate, NDL, tissue loading, CNS, ppO₂, and gas density
* Globe of every dive site, gear and weighting history, SAC from tank pressures, and a logbook you can group and sort
* 57 unlockable sea creatures earned through achievements, each an editable SVG

Scoring logic lives in one module per skill, is versioned so every dive is rescored when the rules change, and is tested against hand-derived synthetic profiles and pinned real dives. CI runs backend tests, frontend lint and build, and both Docker image builds on every PR, and every merge deploys to Railway (API, web app, Postgres, and a volume for photos).

**Tech:** FastAPI · SQLAlchemy · Alembic · PostgreSQL · React · TypeScript · Vite · Tailwind · Recharts · MapLibre GL · Docker · Railway

---

## Other Projects

### FloorSight

**Production monitoring and OEE analytics**

A web application for analyzing production performance using uploaded datasets or live simulations.

Live Demo: https://floorsight-gamma.vercel.app/
* Username: demo@floorsight.app
* Password: demotest

* OEE breakdown into Availability, Performance, and Quality
* Downtime Pareto analysis to identify major losses
* Interactive dashboards and production metrics
* Dockerized deployment on Railway and Vercel

**Tech:** FastAPI · PostgreSQL · React · TypeScript · Docker

### LabelLint

**Dataset quality tools for computer vision**

A toolkit for finding annotation problems before they reach training.

Live Demo: https://labellint.vercel.app/

* Duplicate image detection
* Degenerate or invalid bounding boxes
* Class imbalance detection
* Dataset statistics and validation
* Conversion between YOLO, COCO, and Pascal VOC formats

Built after seeing the same pattern again and again: in most vision projects, the dataset is the bottleneck, not the model.

**Tech:** Python · OpenCV · PyTorch

---

## Professional Background

**Overview AI** — [Application Controls Engineer]
Building AI-powered visual inspection systems for manufacturing.

**Corporate Controls Engineer** (previous)
Supported four US manufacturing plants and led a companywide migration from legacy MES and shopfloor systems to Ignition.

---

## Computer Vision Work

Built proof-of-concept systems with YOLO, OpenCV, PyTorch, and Roboflow, including:

* Gauge readers
* Digital display OCR
* Stack light monitoring
* Tool and component detection
* Vision systems publishing results into Ignition over MQTT

Most of that work was in the less glamorous but more important parts of a vision system:

* Dataset collection
* Annotation quality
* Reducing false positives
* Edge deployment
* Integration with existing industrial systems

---

## Technologies

**Industrial:** PLCs · Ignition · SCADA · MES · MQTT · Industrial Networks

**Software:** Python · TypeScript · FastAPI · React · PostgreSQL · SQLAlchemy · Docker

**Computer Vision:** YOLO · OpenCV · PyTorch · Roboflow
