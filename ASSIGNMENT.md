# DSCI 554 Group Project

> ⚠️ **Important:** Read the [Project Guidelines](#project-guidelines) before you start: they cover team members' responsibilities, attendance, deadlines, and the late policy.

## Description

In your final project, your team will produce a **demo paper** as if submitted to a *visualization* conference. For this, you will write a **research paper**, build and deploy a **demo**, create a **video**, and deliver a **presentation** to the class. The goal of the project is to demonstrate a visual display or system that addresses visualization challenges. As such, this project demonstrates how to apply class concepts to solve visualization challenges and communicate your contributions professionally.

### Visualization Challenges

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

### Artifacts

#### Paper

The paper should be written by the students in their own words in **Overleaf** using the [LNCS format](http://www.springer.com/computer/lncs?SGWID=0-164-6-793341-0) format. AI-generated paper content is not permitted. The paper should be clearly written, concise, and **no more than 5 pages long**. See [PAPER_WRITING_GUIDE.md](PAPER_WRITING_GUIDE.md) for how to get started with Overleaf and what sections to include.

#### Demonstration

This includes the codebase (this repository) and a deployed demonstration on GitHub.io. You must use Vue.js or React with Bootstrap to create the demonstration. Create the Vue/React app at the **top level of this repository**, not in a subdirectory: `package.json` must be in the repository root. The deployed demonstration should be publicly accessible.

The purpose of the demonstration is to show the visual displays your team created to address the visualization challenges. Integrating them into a dashboard or an infographic is a plus, but it is less important and carries less weight in the grade than the challenge visualizations themselves.

Examples with instructions on how to deploy to GitHub.io:
- Vue App: [sample repository](https://github.com/dsci-554/vue-example) and GitHub.io [deployed link](https://dsci-554.github.io/vue-example)
- React App: [sample repository](https://github.com/dsci-554/react-example) and [deployed link](https://dsci-554.github.io/react-example)

#### Video Demo

The video demonstration should be **2 minutes or less**, include a **voice over narrated by the students in their own words**, be **posted on YouTube**, and be publicly accessible. The video itself cannot be generated by AI: AI-generated video, narration, or voice-over scripts are not permitted. Students do not need to appear in the video.

The video must **start with a title slide** showing the project title, the group name, and the authors (team member names). Keep it on screen for a few seconds only: it counts toward the 2 minutes.

A simple way to create the video is to record it with Zoom:

1. In the Zoom desktop app, open **Settings > Recording** and uncheck **Record video during screen sharing**. The recording then contains only the shared screen, with no participant video.
2. Start a Zoom meeting with your team and open the title slide (e.g., the first slide of your presentation in Google Slides) and the deployed demonstration in Chrome. Keep your cameras off.
3. Share the screen showing the title slide.
4. Click **Record** and choose to record on this computer. Introduce the project over the title slide, then switch to the demonstration and walk through it while narrating it.
5. Stop the recording and end the meeting. Zoom saves the recording as an MP4 file.
6. Upload the MP4 file to YouTube and make sure it is publicly accessible.

You do not need to get it right in one take. You can make a longer recording, repeating the parts that did not go well, and then edit it down: cut the mistakes, pauses, and repeated takes with a video editor such as Clipchamp (Windows) or iMovie (Mac), or trim it in YouTube Studio after uploading. The edited video must still be 2 minutes or less.

#### Presentation

The presentation should be **5 minutes long**, created in **Google Slides**, and written by the students in their own words. AI-generated slide content is not permitted. The presentation should feature parts of the Video demonstration played **without audio** rather that a live demonstration.

### Pre-Submission

The pre-submission is a graded milestone on the same [artifacts](#artifacts). The grade is **preliminary**: it shows where you stand, and the final grade comes from the final submission. It uses the same rubric as the final submission ([RUBRIC.md](RUBRIC.md)), accepting Figma placeholders for what is not yet implemented.

The rule for every artifact: **the narrative is final, and Figma placeholders stand in for what is not yet implemented.**

- **Paper:** all sections fully written in prose, no bullet points, with a preliminary title. Describe what is not yet implemented from your Figma design. Figures are captioned screenshots of the deployed site. Cite the major references: the papers closest to your contributions, your data sources, and your main tools (see [PAPER_WRITING_GUIDE.md](PAPER_WRITING_GUIDE.md)).
- **Demonstration:** a site deployed on GitHub.io with a **fully functional reachability map** (challenge 2 in [Visualization Challenges](#visualization-challenges)), including the comparison, the route layer, and the layer and click interaction. Everything else not yet implemented is shown as a Figma placeholder in the site, not a text placeholder.
- **Draft video:** recorded from the deployed site, with final narration. Upload it to YouTube; it can be unlisted as long as the link works.
- **Draft presentation:** in Google Slides, with a final narrative. It is not presented to the class.

To submit, commit the code of the deployed site and replace the placeholder `paper.pdf` with the PDF of your paper, and complete [SUBMISSION.md](SUBMISSION.md) with the links to the GitHub.io site, the Overleaf project, the draft video, and the draft presentation.

### Submission

Update **SUBMISSION.md** with the requested information, written by the students in their own words. AI-generated submission content is not permitted. Students are expected to:

- Commit the code base of the demonstration in this repository
- Replace the placeholder `paper.pdf` in this repository with the PDF of the paper, keeping the file name
- Present to the class as if it were at a conference session.

## Rubric

See [RUBRIC.md](RUBRIC.md) for the grading criteria and point deductions. The pre-submission and the final submission use the same rubric; for the pre-submission, Figma placeholders are accepted for what is not yet implemented.

## Project Guidelines

> ⚠️ **Important:**
>
> - **Team members' responsibilities:** It is strongly suggested to have a team lead for each artifact. All team members should contribute equally to all aspects of the project. Update your contributions in [SUBMISSION.md](SUBMISSION.md) as you do the work, so that nothing is forgotten at submission time.
> - **Attendance:** Students are expected to attend and participate in project labs. Unexcused absences may result in a **5% penalty applied to the final individual project grade**.
> - **Deadlines:** The [pre-submission](#pre-submission) and the final submission must each be completed by their deadline: the project repository must be updated before each deadline.
> - **Late policy:** **There is no late policy: work submitted after the deadline will not be graded**.
> - **Compatibility:** Demonstration is expected to work in Chrome using the latest available Node LTS with up-to-date Node packages.
