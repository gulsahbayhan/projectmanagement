# Intro to Project Management

A practical introduction to project management concepts for AI and software
product work. You will build a shared vocabulary for Agile delivery, understand
how Scrum structures team collaboration, use Kanban to make work visible, and
connect Lean principles to value delivery and continuous improvement.

## Project at a Glance

The project turns delivery principles into a visible, adaptable way of working
for an AI or software team.

```mermaid
%%{init: {"theme":"base","themeVariables":{"fontFamily":"Arial","primaryTextColor":"#172033","lineColor":"#64748B"},"flowchart":{"curve":"basis","nodeSpacing":36,"rankSpacing":52}}}%%
flowchart LR
    Goal[Choose a lightweight<br/>delivery approach]
    subgraph Understand["<b>1. Understand Ways of Working</b>"]
        direction TB
        Values[Agile values<br/>Iteration and feedback]
        Scrum[Scrum]
        Kanban[Kanban]
        Lean[Lean]
        Choice[Select practices<br/>that fit the context]
        Values --> Scrum
        Values --> Kanban
        Values --> Lean
        Scrum --> Choice
        Kanban --> Choice
        Lean --> Choice
    end
    subgraph Apply["<b>2. Make Work Visible</b>"]
        direction TB
        Work[Define valuable work]
        Board[Build a GitHub Projects<br/>Kanban board]
        Policies[Explicit policies<br/>and ownership]
        WIP[WIP limits<br/>and pull flow]
        Work --> Board
        Board --> Policies
        Board --> WIP
    end
    subgraph Improve["<b>3. Inspect and Adapt</b>"]
        direction TB
        Review[Review flow and feedback]
        Change[Choose one improvement]
        Output[Working board and<br/>team delivery agreement]
        Review --> Change --> Output
        Output -. Inspect again .-> Review
    end
    Goal --> Understand --> Apply --> Improve
    classDef goal fill:#172033,color:#FFFFFF,stroke:#172033,stroke-width:2px;
    classDef input fill:#FFFFFF,color:#172033,stroke:#4677A8,stroke-width:1.5px;
    classDef work fill:#FFFFFF,color:#172033,stroke:#3B8A5A,stroke-width:1.5px;
    classDef output fill:#FFFFFF,color:#172033,stroke:#B77A1F,stroke-width:1.5px;
    class Goal goal;
    class Values,Scrum,Kanban,Lean,Choice input;
    class Work,Board,Policies,WIP work;
    class Review,Change,Output output;
    style Understand fill:#F5F9FD,stroke:#9BB8D2,stroke-width:1.5px;
    style Apply fill:#F4FAF6,stroke:#9DC8AD,stroke-width:1.5px;
    style Improve fill:#FFFAEF,stroke:#D7B66B,stroke-width:1.5px;
```

## Learning Objectives

By the end of this repository, you should be able to:

- Explain why Agile project management emphasizes iteration, feedback, and
  adaptation.
- Distinguish Scrum, Kanban, and Lean at a practical level.
- Identify Scrum accountabilities, events, artifacts, commitments, values, and
  pillars.
- Describe how Kanban boards, WIP limits, explicit policies, and flow metrics
  improve team visibility.
- Connect Lean ideas such as value, flow, pull, waste reduction, and continuous
  improvement to AI product work.
- Choose a lightweight project-management approach for a team, product, or
  learning project.

## Learning Path

| File / Folder | Description |
|---|---|
| [**01 - Agile Methodologies**](01-agile-methodologies.md) | Understand Agile values, principles, common methods, and why iterative delivery matters for digital products. |
| [**02 - Scrum**](02-scrum.md) | Learn current Scrum accountabilities, events, artifacts, commitments, values, pillars, and self-check questions. |
| [**03 - Kanban**](03-kanban.md) | Explore visual workflow management, WIP limits, explicit policies, flow metrics, and Kanban boards. |
| [**04 - Lean**](04-lean.md) | Connect Lean principles to waste reduction, continuous improvement, and product delivery. |
| [**05 - Session Handout**](05-session-handout.md) | Use GitHub Projects in groups to manage an AI assistant scenario with a Kanban board. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**assets**](assets/) | Visual aids referenced in the lesson files. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a
> **placeholder**. Replace it including the `< >` brackets with your own value.
> For example, `cd <repo-name>` becomes `cd aipm-intro-to-pm`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete
> this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like:
`git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder

No Python environment is required for this repository.

```bash
cd <repo-name>
```

---

### 5. Open the Lesson Files

Open `README.md` and follow the lesson files in numerical order. The files are
plain Markdown and can be read directly on GitHub or in a local editor.

## References & Further Reading

- [**Agile Manifesto**](https://agilemanifesto.org/): The foundational values
  and principles behind Agile software development.
- [**Scrum Guide**](https://scrumguides.org/scrum-guide.html): The official
  guide to Scrum events, artifacts, commitments, and accountabilities.
- [**Kanban Guide**](https://kanbanguides.org/): A concise reference for Kanban
  systems, flow, WIP limits, and service delivery.
- [**Lean Enterprise Institute: What is Lean?**](https://www.lean.org/explore-lean/what-is-lean/):
  A practical introduction to Lean thinking, value, waste reduction, and
  continuous improvement.
