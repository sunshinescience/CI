# CI

### Quick start
See [here](https://docs.github.com/en/actions/quickstart) for creating your first workflow and how to view the workflow results.

### GitHub actions vs Bamboo:
'steps' here (in the ci.yml file) are called 'tasks' in Bamboo
A 'job' here is a 'stage' in Bamboo

A 'plan' in bamboo is a pipeline

ubuntu is the operating system here in the GitHub actions example

resources with regard to an agent are hardware, e.g., CPU or memory

### To do
Add a step that creates a file with touch, that runs the step command
And make another step that runs the ls command
Another task can be to setup python on this machine

Read through github actions documentation.
Get the VM ready to do the work that's needed.
Here, these are the initialization steps.

### Notes 
What I need to work out: What are the best labels for the agents?
    For example: operating system, software on it (e.g., Python)
    An example is setting up the 'sizes'
    Think of other labels I can make for the agents to make things easier
If everything uses Python, for example, you can install it with a step, or if all of the builds need Python, it might be better to have Python installed on the VM. And then the agent would say it has Python, along with the other attributes it has

- agents have 'attributes' like things that they have (xxs, m/l)

### CI
Continuous integration:
Make code changes, test it locally, and the system does the rest. When someone makes code changes, it builds, tests, and deploys (that is continuous integration).

#### Ways of development
1. One way to work is feature branches (git flow model): pulls master, makes a new branch, makes changes, tests it, then merges it to master
2. Another way is trunk-based development: where people push directly to master


### Notes
Documentation on making continuous integration with GitHub, found here:
https://docs.github.com/en/actions/quickstart

Do a google search for 'github actions python'