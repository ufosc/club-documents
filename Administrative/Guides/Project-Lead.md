# Project Lead Guide

Every project and project group is different, so this guide will not be a detailed series of steps to do, but rather be a list of suggestions and best practices. Remember, you have two goals as a project lead. To finish\* the project and make working on it enjoyable for your team. We believe a team is happy when they can see the progress they make, individual members are able to be productive on their schedule, and everyone gets along. This guide should help you reach those goals.

\* Most projects could go on forever making changes and optimizations, but your team will usually reach a consensus on when to wind down. The great thing about open source is that if a need arises, people can start working on it again.

## Agile Development

The [Agile Manifesto](http://agilemanifesto.org/) is oriented for full-time teams, however there are certainly some ideas that can be incorporated into student teams.

- "Working software is delivered frequently (weeks rather than months)"
	- People will loose enthusiasm for a project if they don't see progress. Set reasonable short-term goals that directly contribute to long-term goals (we will have X feature in two weeks in order to eventually do Y). Also, make sure everyone on your team can contribute to those short-term goals, so they always have something to reach for. These deadlines don't have to be "hard", things happen. Whats important is that your team stays motivated to achieve them.
- "Working software is the primary measure of progress"
	- Don't spend weeks or months trying to get a back-end finished before moving on to the front-end. People like to see the results of their work. Try doing a vertical slice (get just what you need of each layer working for each feature). Not only does this mean you get features working quicker (and get user feedback), your team also gets to find problems with your approach sooner rather than after you "finalize" things.
- "Simplicity-the art of maximizing the amount of work not done-is essential"
	- The more complex the software and the more decisions you lock down, the harder it is to change things (not to mention understand your project). It's often better to "optimize" for making future development easier. Work on low hanging fruit first, delay decisions that lock you down till later (though you will have to make them eventually), and don't worry about performance before you know how well it performs.
- "Regularly, the team reflects on how to become more effective, and adjusts accordingly"
	- Your team has the power to control how you do things. Neither this guide nor anyone else is an expert in your project or your team's dynamic. Feel free to experiment in-order to making your experience better.

## GitHub

GitHub provides excellent [tools for collaboration](https://github.com/features/project-management). This is great for not only managing your current team, but makes it easier for other people (or your future selves) to see what's happening and get involved. Using open development practices is an important part of open source. Keep in mind you probably wont use all of these tools, and that's fine! Do what's best for your team.

- [Issues](https://help.github.com/articles/about-issues/) let your team and users create public discussion for new ideas, tasks, or bugs. Others can add their thoughts and reference other issues. You can decide to assign people to work on the issue. Once you've come to a conclution (such as fixing a bug), you can close the issue, where it will then be archived for future reference.
	- [Labels](https://help.github.com/articles/about-labels/) are used to help categorize issues into things like bugs, enhancements, or being a "good first issue" (to help get beginners started). This makes it easy for people to search for issues they may want to tackle.
- [Milestones](https://help.github.com/articles/about-milestones/) let your team group issues into new releases. This is great for monitoring your short-term goals (see above) and lets you mark when you achieve them.
- [Branches](https://help.github.com/articles/about-branches/) are actually built into Git, but it pays to mention how useful they are here. You can "branch" off of some shared code (usually your dev branch) to work on specific issues. That way only people working on that issue touch the code, so no one else's changes affect yours. Once you're done you can merge your branch back into your shared code so everyone else can use it!
- [Pull Requests](https://help.github.com/articles/about-pull-requests/) by default are used by outside collaborators to submit changes to your project. You can review their code, let them update it, and accept or decline depending on what the project wants.
	- [Code reviews](https://help.github.com/articles/about-pull-request-reviews/) allow your team to make comments directly referencing the code. This is great to catch simple bugs as well as make members more familiar with what others have been working on. You can even set GitHub to require code reviews every time someone tries to merge their code into your shared branch.
- [Projects boards](https://help.github.com/articles/about-project-boards/) are another way of organizing your issues. It allows you to sort issues Kanban style (in a series of specifc columns) such as: TODO, In Progress, and Finished. This can help keep your team stay up-to-date on the progress others are making.

## Clean Architecture

Robust code bases usually meet a handful of ideas.

1. Independent of Frameworks
2. Testable
3. Independent of UI
4. Independent of Database
5. Independent of any external agency

Having code separated into layers that "properly" interact, allows your team to easily make changes without breaking other parts of the code. As a result, people can work on separate parts of the code base without running into issues (which is great for projects with many people). Not all projects should adhere to these principles (for instance it just adds more work to small projects), but keeping in mind the principles of [Clean Architecture](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html) can help your team create features quicker and keep your code healthy in the long run.

## Our Resources

We actually have some useful resources for you and your team to take advantage of. You can of course add to them and make them even better than they are!

- The [Project Template](https://github.com/ufosc/resources/tree/master/project-template) is a set of ideal files for open source projects. Each file includes a template for what to put in it. Check out the [explanation file](https://github.com/ufosc/resources/blob/master/project-template/explanation.md) for information about why you would include each of those in your project.
- [Best Practices](https://github.com/ufosc/resources/blob/master/coding-guidelines/best-practices.md) for coding. Again, they are guidelines not rules, but they are certainly worth considering if you want to improve yourself as a programmer.
- [Coding Guidelines](https://github.com/ufosc/resources/tree/master/coding-guidelines) are style rules both for the general case and specific languages. You can reference them to help keep the code consistent with other projects, or include a modified version of them for in your own repository if your team wants to do things differently. The goal of the guidelines is to make the code as readable as possible, as we believe readability helps people understand the code base quicker and become more productive.
- Finally we have [other resources](https://github.com/ufosc/resources/tree/master/resources) about different programming languages and technology. They include descriptions and helpful links for people to learn about that specific tehcnology. The goal is that all OSC projects can reference them, so if you find a helpful resource, you can add it to the list to let everyone see it.
