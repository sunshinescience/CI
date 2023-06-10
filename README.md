# CI

docs on making continuous integration with GitHub, found here:
https://docs.github.com/en/actions/quickstart


search for github actions python

'steps' here (in the ci.yml file) are called 'tasks' in Bamboo
A 'job' here is a 'stage' in Bamboo

A 'plan' in bamboo is a pipeline

ubuntu is the operating system here in the GitHub actions example

resources with regard to an agent are hardware, e.g., CPU or memory

TODO:
Add other steps tomorrow
A step that creates a file with touch, that runs the step command
And make another step that runs the ls command

Another task can be setup python on this machine

read through github actions documentation
get the VM ready to do the work you need to, this is what we're doing here, initialization steps

________
What I need to work out: What are the best labels for the agents?
    For example: operating system, software on it (e.g., Python)
    An example is setting up the 'sizes'
    Think of other labels I can make for the agents to make things easier
If everything uses Python, for example, you can install it with a step, or if all of the builds need Python, it might be better to have Python installed on the VM. And then the agent would say it has Python, along with the other attributes it has

- agents have 'attributes' like things that they have (xxs, m/l)

