# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change.

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Code of Conduct

### Our Pledge

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age, body
size, disability, ethnicity, gender identity and expression, level of experience,
nationality, personal appearance, race, religion, or sexual identity and
orientation.

### Our Standards

Examples of behavior that contributes to creating a positive environment
include:

- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

## I Want To Contribute

### Reporting Bugs

#### Before Submitting a Bug Report

A good bug report shouldn't leave others needing to chase you up for more information. Therefore, we ask you to investigate carefully, collect information and describe the issue in detail in your report. Please complete the following steps in advance to help us fix any potential bug as fast as possible.

- Make sure that you are using the latest version.
- Determine if your bug is really a bug and not an error on your side e.g. using incompatible environment components/versions (Make sure that you have read the [documentation](). If you are looking for support, you might want to check [this section](#i-have-a-question)).
- To see if other users have experienced (and potentially already solved) the same issue you are having, check if there is not already a bug report existing for your bug or error in the [bug tracker](issues?q=label%3Abug).
- Also make sure to search the internet (including Stack Overflow) to see if users outside of the GitHub community have discussed the issue.
- Collect information about the bug:
- Stack trace (Traceback)
- OS, Platform and Version (Windows, Linux, macOS, x86, ARM)
- Version of the interpreter, compiler, SDK, runtime environment, package manager, depending on what seems relevant.
- Possibly your input and the output
- Can you reliably reproduce the issue? And can you also reproduce it with older versions?

#### How Do I Submit a Good Bug Report?

> You must never report security related issues, vulnerabilities or bugs including sensitive information to the issue tracker, or elsewhere in public. Instead sensitive bugs must be sent by email to <>.

We use GitHub issues to track bugs and errors. If you run into an issue with the project:

- Open an [Issue](/issues/new). (Since we can't be sure at this point whether it is a bug or not, we ask you not to talk about a bug yet and not to label the issue.)
- Explain the behavior you would expect and the actual behavior.
- Please provide as much context as possible and describe the _reproduction steps_ that someone else can follow to recreate the issue on their own. This usually includes your code. For good bug reports you should isolate the problem and create a reduced test case.
- Provide the information you collected in the previous section.

### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion for CONTRIBUTING.md, **including completely new features and minor improvements to existing functionality**. Following these guidelines will help maintainers and the community to understand your suggestion and find related suggestions.

#### Before Submitting an Enhancement

- Make sure that you are using the latest version.
- Read the [documentation]() carefully and find out if the functionality is already covered, maybe by an individual configuration.
- Perform a [search](/issues) to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.
- Find out whether your idea fits with the scope and aims of the project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Keep in mind that we want features that will be useful to the majority of our users and not just a small subset. If you're just targeting a minority of users, consider writing an add-on/plugin library.

#### How Do I Submit a Good Enhancement Suggestion?

Enhancement suggestions are tracked as [GitHub issues](/issues).

- Use a **clear and descriptive title** for the issue to identify the suggestion.
- Provide a **step-by-step description of the suggested enhancement** in as many details as possible.
- **Describe the current behavior** and **explain which behavior you expected to see instead** and why. At this point you can also tell which alternatives do not work for you.
- You may want to **include screenshots and animated GIFs** which help you demonstrate the steps or point out the part which the suggestion is related to. You can use [this tool](https://www.cockos.com/licecap/) to record GIFs on macOS and Windows, and [this tool](https://github.com/colinkeenan/silentcast) or [this tool](https://github.com/GNOME/byzanz) on Linux.
- **Explain why this enhancement would be useful** to most CONTRIBUTING.md users. You may also want to point out the other projects that solved it better and which could serve as inspiration.

### Pull Request Process

#### 1. Fork the Repository

First, you need a personal copy of the project to make changes.

- Navigate to the original project repository on GitHub.
- Click the **Fork** button in the upper-right corner of the page.
- Select your personal GitHub account as the destination.

#### 2. Clone the Repository Locally

Next, copy your forked repository from GitHub onto your local machine.

- Click the green **Code** button on your forked repository page.
- Copy the HTTPS or SSH URL provided.
- Open your terminal and run the following commands:

```
# Clone your personal fork (replace with your username and repo name)
git clone https://github.com

# Navigate into the project directory
cd PROJECT_NAME
```

#### 3. Configure the Upstream Remote

To easily keep your local files updated with the original repository's changes, add it as an upstream remote reference.

```
# Add the original repository as 'upstream'
git remote add upstream https://github.com

# Verify that your remotes are correctly set up
git remote -v
```

#### 4. Create a Feature Branch

Always isolate your work in a dedicated branch. Never develop directly on the `main` or `master` branch.

```
# Fetch the latest updates from the original repository
git fetch upstream

# Create and switch to a new feature branch
git checkout -b feature/your-descriptive-feature-name
```

#### 5. Commit Your Changes

Make your code modifications, stage them, and write clear, concise commit messages.

```
# Track and stage your modified files
git add .

# Create a local commit with an explicit, descriptive message
git commit -m "feat: add descriptive message of what you changed"
```

Ensure any install or build dependencies are removed or excluded before doing a
build and commit changes.

#### 6. Push to Your Fork

Upload your local branch and commits up to your own GitHub remote workspace (`origin`).

```
# Push your feature branch to your GitHub fork
git push origin feature/your-descriptive-feature-name
```

#### 7. Open a Pull Request (PR)

Submit your proposed code changes back to the original repository for review.

1. Go to the original project repository on GitHub and change to `development` branch.
2. You will see a prominent yellow banner reading **"Compare & pull request"**. Click it.
3. Ensure the **base repository** points to the original project and the **head repository** points to your fork and feature branch.
4. Provide a clear title and detail your updates in the description template.
5. Click **Create pull request**.
6. You may merge the Pull Request in once you have the sign-off of two other developers, or if you
   do not have permission to do that, you may request the second reviewer to merge it for you.

---

### Keeping Your Branch Updated

If your PR takes a while to review and the original repository gets updated, sync your feature branch to prevent merge conflicts:

```
# Pull down changes from the original repository
git checkout main
git pull upstream main

# Merge updates into your feature branch
git checkout feature/your-descriptive-feature-name
git merge main

# Push the synchronized updates back to your fork
git push origin feature/your-descriptive-feature-name
```
