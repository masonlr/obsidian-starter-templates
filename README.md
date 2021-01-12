# Obsidian Starter Templates

**Obsidian Starter Templates** is a reference for using [Obsidian](https://obsidian.md/).

If you've tested out [Obsidian](https://obsidian.md/) and worked through the "Obsidian Help" folder, you might be looking for practical strategies to apply associative notes in your daily work.

**Obsidian Starter Templates** gathers examples from the Obsidian [community](https://forum.obsidian.md/). Its broader aims are to uncover and communicate:

1. How others use backlinks and various markdown tricks,
2. Why these techniques work.

The initial example covers how an academic [researcher](https://github.com/masonlr/obsidian-starter#researcher) might choose to approach Obsidian.

## Getting started

**Starter Templates** contains template vaults. To get started:

1. Clone the repository and open a vault folder in Obsidian using the "Open another vault" sidebar button.

## Templates

### Researcher

The [researcher/](./researcher) template suits a case where you are juggling multiple research projects: for example, reading several books and research papers simultaneously and maintaining multiple collaborations with other researchers. It's nice to have a starter template to experiment with ideas, even though backlinks and associative thinking encourage you to avoid hierarchies and rigid hierarchical structures: see for example Andy Matuschak's [evergreen notes](https://notes.andymatuschak.org/Evergreen_notes), [taxonomy of note types](https://notes.andymatuschak.org/Taxonomy_of_note_types) and [note-link-janitor](https://github.com/andymatuschak/note-link-janitor) project.

#### Example network

<img src="assets/researcher.png" style="zoom:50%;" />

The template is intended to be modular. A minimal use could include [scratch/](https://github.com/masonlr/obsidian-starter#scratch) and [concepts/](https://github.com/masonlr/obsidian-starter#concepts), then later expand to [projects/](https://github.com/masonlr/obsidian-starter#projects) and [people/](https://github.com/masonlr/obsidian-starter#people). The intended structure is given by the following tree:

#### [scratch/](./researcher/scratch/)

The scratch folder is an area for messy, low-friction daily free-form planning and logging of ideas, i.e. [scratch/](./researcher/scratch/) will store content generated using the Obsidian "daily notes" feature. Daily notes can be created using the "Open today's note" action: this will create a new markdown file that follows the date-stamped name convention `YYYY-MM-DD.md`.

**Tip:** Set a keyboard shortcut to quickly go to the day's note. For example, set `cmd+T` to "Open today's note" in the Hotkeys settings.  
**Tip:** Create a rigid for daily notes by specifying a template markdown file, though a blank template may encourage free-form thinking.

After a few days, daily notes will build up as follows:

- [2020-05-24.md](./researcher/scratch/2020-05-24.md)

- [2020-05-25.md](./researcher/scratch/2020-05-25.md)

- [2020-05-26.md](./researcher/scratch/2020-05-26.md)

  **TIP:** Keep a free-form record of what you're reading, doing and thinking about by linking to concepts and books: this way backlinks in each concept will show that dates on which work was done. Example in [2020-05-24.md](./researcher/scratch/2020-05-24.md):

  ```markdown
  Read about [[A concept]] in [[Saini (2017) – Inferior]]
  ```

  When later reviewing [A concept.md](./researcher/concepts/A%20concept.md), backlinks will show that you were thinking about it on a particular date ([2020-05-24.md](./researcher/scratch/2020-05-24.md)).

  **TIP:** Use tags such as `#backlog` and `#priority` for simple Kanban-style task tracking, see [Distributed idea tracking](https://github.com/masonlr/obsidian-starter-templates#distributed-idea-tracking).

#### [concepts/](./researcher/concepts/)

Folder for "evergreen" concept notes (see Andy Matuschak's [evergreen notes](https://notes.andymatuschak.org/Evergreen_notes)).

- [A concept.md](./researcher/concepts/A%20concept.md)

  A example concept note.

  **TIP:** In a link, it's clearer to read `[[A concept]]` than `[[a-concept]]`, so the filename uses white spaces here and sentence case.

  **TIP:** The filename is more important than the level-one heading. Use a filename appropriate for linking, but use a longer more descriptive level-one heading. Example in [A concept.md](./researcher/concepts/A%20concept.md) where the level-one heading is longer than the filename:

  ```markdown
  # A new concept that is useful
  ```

#### [projects/](./researcher/projects/)

Link ideas, concepts and people to projects.

- [Project A.md](./researcher/projects/Project%20A.md)

  **TIP:** Link to projects from daily notes to keep an informal record of progress. Example in [2020-05-24.md](./researcher/scratch/2020-05-24.md):

  ```markdown
  Got started on ideas about [[Main concept]] for [[Project C]].
  ```

  Project backlinks will then show dates that it was worked on.

  **TIP:** Add links to people and details of there involvement. Example in [Project A.md](./researcher/projects/Project%20A.md):

  ```markdown
  ## People

  - [[Supervisor]]
  - [[Collaborator A]]
  - [[Collaborator B]] might be interested.
  ```

- [Project B.md](./researcher/projects/Project%20B.md)

- [Project C/](./researcher/projects/Project%20C/)

  If a project becomes more complex, it might turn into a folder with many attached concept notes.

  - [Project C.md](./researcher/projects/Project%20C/Project%20C.md)
  - [Main concept.md](./researcher/projects/Project%20C/Main%20concept.md)
  - [Another concept.md](./researcher/projects/Project%20C/Another%20concept.md)

#### [people/](./researcher/people/)

Keep track of interactions with collaborators. If you're doing a research project, you might also have a file for your adviser/supervisor.

- [Collaborator A.md](./researcher/people/Collaborator%20A.md)
- [Collaborator B.md](./researcher/people/Collaborator%20B.md)
- [Supervisor.md](./researcher/people/Supervisor.md)

**TIP:** Link to a person from anywhere if there is an association. You could link from a concept. Example in [A concept.md](./researcher/concepts/A%20concept.md) links to a person from a concept:

```markdown
[[Collaborator A]] has a good idea about this, but [[Supervisor]] thinks that this is wrong.
```

**TIP:** To keep a record of interactions you could link from the daily log. Example in [2020-05-25.md](./researcher/scratch/2020-05-25.md) links from a potential task to a person:

```
#priority Meet with [[Collaborator B]] to discuss ideas.
```

#### [books/](./researcher/books/)

Keep a record of important books here. Each book page could link to a set of relevant concept notes, rather than containing content. If you're undertaking a research project, you could also add an `articles/` folder.

- [Csikszentmihalyi – Flow.md](<./researcher/books/Csikszentmihalyi%20(2008)%20%E2%80%93%20Flow.md>)

  **TIP:** Link to concept pages rather than writing directly in a book page (see Andy Matuschak's [taxonomy of note types](https://notes.andymatuschak.org/Taxonomy_of_note_types)). Example in [Csikszentmihalyi – Flow.md](<./researcher/books/Csikszentmihalyi%20(2008)%20%E2%80%93%20Flow.md>) links from a book to a concept:

  ```markdown
  - One of the chapters focused on [[A concept]]
  ```

  **TIP:** Link from concept pages to book pages. Example in [A concept.md](./researcher/concepts/A%20concept.md):

  ```markdown
  - [[Saini (2017) – Inferior]] described it like this, but [[Csikszentmihalyi (2008) – Flow]] described it like that.
  ```

- [Saini – Inferior.md](<./researcher/books/Saini%20(2017)%20%E2%80%93%20Inferior.md>)

  **TIP:** Link from PDF pages to book pages:

  ```markdown
  - [[Saini (2017) - Inferior.pdf#page=40]] described it.
  ```

#### [tools/](./researcher/tools/)

Think about the tools you're currently using, search for new tools, write notes about what you've learnt.

- [The first tool.md](./researcher/tools/The%20first%20tool.md)

#### [meta/](./researcher/meta/)

Question your approaches here and keep a record of insights and meta concepts.

- [TIL.md](./researcher/TIL.md)

  Use to record today-I-learned ([TIL](https://dictionary.cambridge.org/dictionary/english/til)) style ideas. Example in [2020-05-26.md](./researcher/scratch/2020-05-26.md) links two concepts:

  ```markdown
  [[TIL]] Some interesting idea that stood out. It changed how I thought about [[A concept]] in relation to [[Another concept]].
  ```

  **TIP:** Backlinks to [TIL.md](./researcher/TIL.md) will show a record of when concepts were learnt.

- [Strategy.md](./researcher/meta/Strategy.md)

- [Wins.md](./researcher/meta/Wins.md)

  **TIP:** Keep a record of any milestones or positive feedback.

#### [images/](./researcher/images/)

(optional) You can set a dedicated folder to handle all image uploads: the folder will hold a copy of all images dragged onto Obsidian notes.

- [panda.jpg](./researcher/images/panda.jpg)

  **TIP:** When renaming an image, all links to it will be automatically updated.

### Distributed idea tracking

Rather than maintaining a list of tasks, distribute the tags across all files so that tags are placed alongside content. Tags can be used to replace simple Kanban-style task tracking. Use whatever tag system works for you – an example idea tags could include:

- `#next`: Must be done next.

  **TIP:** Limit to 2 or 3 instances for a work-in-progress limit.

- `#backlog`: Should be done in the future.

- `#priority`: Should be done soon.

- `#irk`: Must be done soon, but annoying or getting in the way.

- `#lateral`: Interesting left-field idea that may or may not lead anywhere. High-risk, high-reward.

- `#question`: Something uncertain. Plays the role of Wikipedia's [citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed).

Once an idea has been explored or a task has been finished, delete the tag or add

- `#done`: Done

Kanban with embeded queries:

  ```markdown
  |              |                 |           |
  | ------------ | --------------- | --------- |
  | ![[Backlog]] | ![[InProgress]] | ![[done]] |
  ```

  Example in `Backlog.md`:

  ````markdown
  ```query
  tag:backlog
  ```
  ````

#### Task lists

[Markdown task lists](https://help.github.com/en/github/managing-your-work-on-github/about-task-lists) work well in WYSIWYG editors such as [Typora](https://typora.io/). WYSIWYG editing is on the [Obsidian roadmap](https://trello.com/b/Psqfqp7I/obsidian-roadmap), so may well become a better option than a tag based system.

### Referencing

For one-off references, pasted links work fine. Example in [A concept.md](./researcher/concepts/A%20concept.md):

```markdown
This concept only appeared once, so just paste link.
https://en.wikipedia.org/wiki/Mental_state
```

If a link occurs multiple times, it might be appropriate to use markdown footnotes and gather a reference list. Example in [A concept.md](./researcher/concepts/A%20concept.md):

```markdown
This link appears many times,[^repeated] so maybe use a footnote.
A reference[^repeated] had an even different idea to [[Csikszentmihalyi (2008) – Flow]].

[[Collaborator A]] has a good idea about this, but [[Supervisor]] thinks that this is wrong.
I need to check.[^repeated]

## References

[^repeated]: Flow (psychology): https://en.wikipedia.org/wiki/Flow_(psychology)
```

## References

- Obsidian: https://obsidian.md/
- Matuschak, A. Evergreen notes: https://notes.andymatuschak.org/Evergreen_notes
- Matuschak, A. Note-link Janitor: https://github.com/andymatuschak/note-link-janitor
- Matuschak, A. Taxonomy of note types: https://notes.andymatuschak.org/Taxonomy_of_note_types
