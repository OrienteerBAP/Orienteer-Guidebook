# Business Process Management

Orienteer Business Process Management module is currently in beta testing and it's not available `master` branch.
You can get access to BPM module:
* On GitHub in `bpm` branch: https://github.com/OrienteerBAP/Orienteer/tree/bpm
* By Docker image with tag `bpm-latest`: https://hub.docker.com/r/orienteer/orienteer/tags/

Instructions bellow are for experienced users only! We do understand what quality and user-friendliness means: so we are working on bring good value to master stream.

## Creation of a process definition

Orienteer embedded BPM Modeler is not mature enough. So make sure that you are modeling your BPM process in Camunda modeler: https://camunda.org/bpmn/tool/

Once BPMN file is ready, go to your Orienteer installation and create new document of type BPMProcessDefinition. After creation of a process definition: drag and drop your file into editor and click save on left-bottom corner. Make sure that `key` property is equal to `id` of your process in BPMN file.

## Starting a process

Currently, there is no good place to start a process. So it's recommended to use devutils console for that. To make that happend: go to the list of installed modules (OModule) and enable `devutils`. Then you can navigate your brawser to `/tools` page.

So, to start newly created process just execute the following command:

```java
Packages.org.camunda.bpm.BpmPlatform.getDefaultProcessEngine().getRuntimeService().startProcessInstanceByKey('business-process-key')
```
 where `business-process-key` is described below key of a process.
 
 That's all: you process has been started. If you had some user-tasks: they will be available on users profiles.
 
 ## Support of forms
 
 Orienteer doesn't support Camunda's forms described here: https://docs.camunda.org/manual/7.5/user-guide/task-forms/ Instead of Camunda forms, Orienteer supports its own type of keys.
 Format: `orienteer:<Schema Class Name>:<Variable>`
 
 Schema Class Name - name of OClass to be used for creation a new document. It's optional of variable has already contain required document to be shown
 Variable - name of variable to store a newly created document or to take that document from.
 
 Example: `orienteer:OFunction:function`
 First form with this key will create a document of class OFunction and propose a user to enter required information to it. Then document will be stored in variable `function`. 
 Second and later forms with exactly such key will propose user to do something with already created document.
 