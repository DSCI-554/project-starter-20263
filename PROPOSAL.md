# DSCI 554 Group Project: Proposal

## Description

The proposal is the first milestone of the group project described in [ASSIGNMENT.md](ASSIGNMENT.md). Its purpose is to **define your contributions** before you write prose or code. By the end of the proposal, your team should be able to state exactly what visualization(s) you will contribute to the team's dashboard, show what each one will look like as an integrated part of that dashboard, and outline the paper that will present them.

The proposal has three parts: a **contributions statement**, a **paper in bullet points**, and **renderings of the contributions**.

### Scope

Your contributions must be visualizations that are **not stock or existing charts**. A contribution is a visual display your team designs to address a specific visualization challenge, not a chart type that a charting library already provides.

Examples of in-scope contributions include:

- Complex visualizations integrated in a dashboard, such as interactive **reachability maps** or **isochrone maps**
- Visualizations of **GPS traces** that change over location and time
- **Dasymetric mapping**

The following are **out of scope**:

- **Visualizing aggregate data with basic charts.** A dashboard of bar, line, pie, or scatter charts, or a basic choropleth, over summarized data is not a contribution, no matter how polished it is.
- **Dashboards that simply visualize readily available datasets** (e.g., common Kaggle datasets) without addressing a specific visualization challenge. Using an easy-to-access dataset is fine, but the dataset itself does not make the dashboard a contribution.
- **Displays for data exploration.** A set of filters and linked charts that lets users browse a dataset without addressing a specific visualization challenge is not a contribution.

A quick test for each contribution: if it could be produced by picking a chart type in a charting library and passing it your data, it is out of scope. Basic charts may still appear in your dashboard as supporting views, but they do not count as contributions.

### Requirements

#### Contributions

State your contributions as a short numbered list, as they will appear at the end of your paper's Introduction. For each contribution, provide:

- **Name:** a short name for the visualization.
- **Visualization challenge:** the specific challenge it addresses, and for whom.
- **What is new:** how it differs from stock charts and from the existing work you will cite.
- **Data:** the data it requires, whether your team already has access to it, and—if not—how you will obtain or generate suitable data. Data availability is not a limitation: you may use synthetic data when real-world data is unavailable.
- **Interaction:** how the user interacts with it, and how it changes in response (e.g., over location, over time).

#### Paper

The paper should be written in **Overleaf** using the [LNCS format](http://www.springer.com/computer/lncs?SGWID=0-164-6-793341-0) format. See [PAPER_WRITING_GUIDE.md](PAPER_WRITING_GUIDE.md) for the sections to include and what each one should cover.

For the proposal, the paper must be completed as follows:

- **Title:** provide a preliminary title
- **Abstract:** Bullet points.
- **Introduction:** Bullet points, ending with the numbered list of contributions.
- **Related Work:** Bullet points, grouped by theme, each stating how your contributions differ.
- **Data**: Bullet points describing the data sources and availability. If suitable real-world data is unavailable, explain how you will generate or use synthetic data; lack of access to real-world data does not prevent you from pursuing a contribution.
- **Dashboard Design:** Bullet points describing the overall dashboard layout and how the contributions fit together.
- **Design and Implementation:** Bullet points, organized by contribution.
- **Usage Scenarios and Results:** Bullet points, with at least one scenario per contribution.
- **Conclusion**: Bullet points.
- **References:** Must include the major references for each contribution.

#### Renderings

Provide **at least one rendering of each contribution**, included as a figure in the paper with a caption. Also include a rendering of the **overall dashboard** to demonstrate its layout and how the contributions fit together. A rendering may be a hand sketch, a Figma mockup, or a screenshot of an early prototype. Each contribution rendering must show:

- **The visual encoding:** what the marks are and what the position, color, size, and shape represent.
- **The interaction:** what the user can do and what changes as a result. Use annotations or several frames if a single image cannot show this.
- **The context:** where the contribution sits in the dashboard.

Screenshots of existing tools, or of stock charts standing in for your design, are not renderings of your contribution.

### Submission

Update **SUBMISSION.md** with the requested information. Students are expected to:

- Complete the project information in the [SUBMISSION.md](SUBMISSION.md) file, including the links to the Overleaf project and the PDF of the paper.
- Include the contributions, the bullet-point sections, and the renderings in the paper.

## Rubric

| **Category** | **Excellent (4–5 pts)** | **Satisfactory (2–3 pts)** | **Needs Improvement (0–1 pts)** |
|--------------|--------------------------|------------------------------|----------------------------------|
| **Contributions** | Contributions are specific, clearly stated, and each addresses a visualization challenge. All are in scope: none is a stock or existing chart. | Contributions are stated but vague, or some rely on stock charts or data exploration. | Contributions are missing, or are out of scope (basic charts of aggregate data, data exploration displays). |
| **Renderings** | Every contribution has a rendering that clearly shows its visual encoding, interaction, and place in the dashboard. | Renderings are present but incomplete: a contribution is missing one, or encoding or interaction is unclear. | Renderings are missing, or show existing tools or stock charts in place of the contributions. |
| **Paper: Outline** | All sections are present in LNCS format with bullet points that give a clear, logical outline. Design and Usage Scenarios are organized around the contributions. | Sections are present but bullet points are thin or loosely connected to the contributions. Minor LNCS formatting issues. | Sections are missing, or the outline shows no evidence of project planning. |
| **Paper: Related Work & References** | Major references are included for each contribution, and the outline states how each contribution differs from existing work. | References are adequate but limited, or the difference from existing work is unclear. | References are missing or irrelevant. |

## Project Guidelines

- Students are expected to attend and participate in project labs. Unexcused absences may result in a **5% penalty applied to the final individual project grade**.
- Late policy: **There is no late policy: work submitted after the deadline will not be graded**.
