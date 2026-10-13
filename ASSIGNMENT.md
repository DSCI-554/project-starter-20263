# DSCI 554 Group Project

## Description

In your final project, your team will produce a **demo paper** as if submitted to a *visualization* conference. For this, you will write a **research paper**, build and deploy a **demo**, create a **video**, and deliver a **presentation** to the class. The goal of the project is to demonstrate a visual display or system that addresses a visualization problem or challenge. As such, this project demonstrates how to apply class concepts to solve visualization challenges and communicate your contributions professionally.

### Requirements

#### Paper

The paper should be written in **Overleaf** using the [LNCS format](http://www.springer.com/computer/lncs?SGWID=0-164-6-793341-0) format. The paper should be clearly written, concise, and **no more than 5 pages long**. See [PAPER_WRITING_GUIDE.md](PAPER_WRITING_GUIDE.md) for the sections to include.

#### Demonstration

This includes the codebase (this repository) and a deployed demonstration on GitHub.io. You must use Vue.js or React with Bootstrap to create the demonstration. The deployed demonstration should be publicly accessible.

Examples with instructions on how to deploy to GitHub.io:
- Vue App: [sample repository](https://github.com/dsci-554/vue-example) and GitHub.io [deployed link](https://dsci-554.github.io/vue-example)
- React App: [sample repository](https://github.com/dsci-554/react-example) and [deployed link](https://dsci-554.github.io/react-example)

#### Visualization Challenges

Your project addresses **two visualization challenges**, each stated explicitly in the paper:

1. **Primary challenge (your own).** The challenge your topic and display are built around, chosen by your team. Your main research, related work, and Results go here.
2. **Reachability challenge (required for every team).** A **reachability map of one city**, built on your own domain and data, in **deck.gl** (with a Mapbox or MapLibre basemap) inside your Vue/React + Bootstrap app. D3 may be used for legends and linked charts. Building the map itself with D3 or Canvas is allowed only if you justify it in the paper. It is a side contribution if your primary challenge is unrelated, or the main contribution if your topic is about access or travel. Either way it gets its own subsection in Results. The name is descriptive, not an established term: the isochrone and accessibility literature covers the pieces, so your related work should state the gap.

The point of this map is to make a *computed* measure visible, not to filter and chart a table. Pick something worth asking of a city, for example walking time to parks and green spaces from each census block group, or driving time to basketball venues (arenas, college and high-school gyms, tournament sites, public courts) at game time versus off-peak. These are examples; choose your own.

The reachability map must include:

1. **Computed reachability.** A travel-time, distance, or hop measure derived from network or relational data (routing, schedules, flows, OD pairs), not a column that arrives in the source. Precomputing offline and shipping static JSON/CSV is expected.
2. **One mode and one level, matched to what is being reached.** Walking suits parks and green spaces, driving suits regional venues. Justify the mode and the travel-time threshold, and use a unit finer than the city (census tract, block group, or grid cell) for the result.
3. **A comparison, not a single surface.** Show at least two conditions or groups on the same measure, for example peak versus off-peak, or neighborhoods grouped by income. If you model rush hour, a documented average slowdown applied to free-flow routing times is enough, and it must be disclosed as an estimate.
4. **A route or path layer** showing the network behind the numbers, with a plan for overplotting.
5. **Layer and click interaction** (toggle layers, click a destination to see its catchment). Anything beyond that is optional.
6. **A named reachability challenge** (see [PAPER_WRITING_GUIDE.md](PAPER_WRITING_GUIDE.md)) with the design decision that addresses it.
7. If you use synthetic data (for example OD flows built from survey data, or an estimated rush-hour slowdown), disclose its derivation and validation.

#### Pre-Submission

The pre-submission is graded and uses the **same artifacts as the final** (paper and demo). The paper is **final in form**, with the work not yet done written as a plan:

- **Demo:** deployed to GitHub.io with the final layout. Placeholders for every visualization except the reachability map, which works end to end for the one city, including the comparison and the route layer.
- **Paper:** final LNCS structure, all sections written in prose (not bullets), as if final. Anything you have not done yet is written as a **plan** (what you will do, with which data, methods, and measures) instead of as results; only what exists in the demo and the display design is described as done. Use **marked placeholders for tables and images** (a caption and a note on what it will show). The Results section has a subsection for each challenge, with the plan for each.
- **SUBMISSION.md:** completed as for the final.

The final grade is pending the paper's results and the demo upgrade, plus the video and presentation. See [RUBRIC.md](RUBRIC.md).

#### Video Demo

The video demonstration should be **2 minutes or less**, include a **voice over**, be **posted on YouTube**, and be publicly accessible.

#### Presentation

The presentation should be **5 minutes long** and created in **Google Slides**. The presentation can feature parts of the Video demonstration played **without audio**.

### Submission

Update **SUBMISSION.md** with the requested information. Students are expected to:

- Commit the code base of the demonstration in this repository
- Present to the class as if it were at a conference session.

## Rubric

See [RUBRIC.md](RUBRIC.md) for the grading criteria and point deductions.

## Project Guidelines

- Students are expected to attend and participate in project labs. Unexcused absences may result in a **5% penalty applied to the final individual project grade**.
- Project repository must be updated before the deadline (last day of class 11:59 PM)
- Late policy: **There is no late policy: work submitted after the deadline will not be graded**.
- Demonstration is expected to work in Chrome using the latest available Node LTS with up-to-date Node packages

