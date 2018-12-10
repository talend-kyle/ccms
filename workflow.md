# Workflow

To work on any file in the CCMS, you must lock it. You can lock a file by right-clicking it and selecting __Lock__.

A locked object appears bold and blue. Another user will see a locked object as red.

A locked file can only be changed by the person who locks that file. Before anyone else can work on that file you must release it but right-clicking and selecting __Release__.

You can lock and open a topic at the same time by right-clicking a topic then selecting __Edit__.

## Locking a topic without changing a topic

If you lock a document, after you release it, the repository saves a revision. This is unnecessary. Instead of clicking __Release__, right-click and select __Replace with server version__.

## Undoing a saved change

You changed a topic and clicked __Save__, but you don't want that change. Use the __Replace with server revision__ option. This function replaces the changes you saved and releases the document.

## Releasing documents

After you click __Save__, you commit the change to the repository by right-clicking the topic then selecting __Release__. it is good practice to always leave a release message, which should follow the same guidelines as a Git commit message.

## Document status

Every object in the CCMS has a status. The workflow of an object is a list of statuses and the order in which the object proceeds through the statuses in the workflow.

To change a document status, unlock it first, then right-click it and select __Change status__.

![changestatus](./images/changeStatus.png)

The workflow GUI opens. Here, you can see the specific object workflow. 

![workflow](./images/workflow.png)

When you select a new status from the GUI, the change is reflected beside the object in the CCMS.

![changedstatus](./images/changedStatus.png)

|Status | Description | After |
|---    | --- | --- |
|Authoring:contribute | SME or external contributor | Must get PM review |
|Authoring:PM approval | Owner must approve or reject | Authoring:work OR authoring:reject|
|Authoring:peer review | Peer review from another writer | Authoring:work|
|Authoring:done|Work is complete|Authoring:work (if needed)|

You can leave change status comments whenever you change the status.

Statuses of objects higher in the document hierarchy cannot change before the dependents. For example, you cannot change a map to `done` unless all topics nested under the map are also in `done`.

![notdone](./images/cannotChangeStatus.png)

These status dependencies prevent the parent from moving to a status ahead of its children. Likewise, when you change the status of a topic from `done` to `work`, the parent will also change.

![images](./images/parentChange.png)

### Assignments and assignees

Assignments are defined in the `roles.xml` file in the administration tool.

To assign a person to a topic, right-click the topic and click __Assign__.

![assign](./images/assign.png)

The assign dialog opens. Here you can select writers, subject-matter experts, reviewers, etc. to topics based on the roles defined by the administrator in the `roles.xml` file.

![assign](./images/assingTo.png)

Objects that are assigned to you appear in the __Todo__ tab. 

![todo](./images/todoList.png)

Notice in the dialog above that some objects are listed more than once. They correspond to the same objects in different versions. When you change the status of an object that you are working on from `work` to `review`, the object is removed for you active todo list and it is placed in your __Incoming list__.