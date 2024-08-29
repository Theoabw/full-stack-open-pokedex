## Common CI Steps and Tools in Python Ecosystem

For each of these steps, the maintainers of a Python project can choose to rely on the following:

1. Linting: Ruff is a very fast Python linter and formatter that encompasses several other tools. More traditional options include flake8 and pylint.

2. Testing: Pytest is the de facto testing framework for Python. The default unittest module is also very popular and widely used, especially in older projects.

3. Building: setuptools is the standard for building and packaging. It's always used along with wheel for making distributable packages. For projects with compiled extensions, tools like cibuildwheel can be used for creating cross-platform wheels.

## Alternatives to Jenkins and GitHub Actions

Some alternatives to GitHub Actions and Jenkins include:

1. GitLab CI: This is tightly coupled with GitLab and forms a full DevOps platform.
2. CircleCI: It's well-regarded for its speed and parallel testing capabilities.
3. Buildkite: Self-managed, runs on your own infrastructure but easier to set up than Jenkins
4. Drone: Container-native CI that is easy to self-host.

## Self-Hosted vs. Cloud-Based CI

Whether to use self-hosted or cloud-based CI depends on the following:

1. Security Requirements: The need for full control over the environment may be dictated by whether the application will handle sensitive data or has compliance requirements that are particularly strict.

2. Expertise of the Team Members: Cloud-based solutions generally come with fewer maintenance needs and, therefore, require lesser expertise for handling. This would be an added advantage to a small team of 6 persons.

3. Scalability Requirements: Cloud-based CI is usually easier to scale, which may be a consideration if the team is likely to grow very fast or if demands are likely to fluctuate.

4. Cost: For a small team, a cloud-based solution may be cheaper to start off with, since there is no upfront cost of setting up self-hosted infrastructure.

Ultimately, it is likely that for a team of 6 people in this project with a Python application nearing release, a cloud-based CI solution can be an optimal choice when balancing considerations of ease of use, cost, and scalability.