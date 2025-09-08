## GitHub Actions Building Blocks

There are three building blocks and these are workflows , jobs and within jobs we have steps.

* Workflows are defined **at the repository level** that means whenever we want to create a workflow , we have to create within a repository.

  * They also define which **triggers** actually start the workflow , this is not *the neither job nor at the step level*, but rather at the workflow level.
  * Workflows are composed of one or more jobs.
* Jobs are defined at the workflow level.

  * we cannot create jobs outside of workflows, and they also define in which **execution environment** they are run this can be Linux , Windows or Mac.
  * They are composed of one or more steps and by **default jobs are run in parallel**.That means if you create ten jobs and you do not specify any dependencies between these jobs, they will all start at the same time whenever the workflow is triggered.
* Steps are defined at **the job level** and they define the actual script or GitHub action that will be executed once that step is then run.By default , the steps run sequentially, and actually the by default here is superfluous because steps will always run sequentially.

GitHub action is the feature offered by GitHub , the whole thing , the workflows , the custom actions.
