# Hacker News Workflow

![workflow](https://github.com/user-attachments/assets/1c9ea07a-5f84-4658-9be4-70518682228d)


## Overview
This lesson guides you through building a small workflow that retrieves 10 articles about automation from Hacker News. The workflow consists of five steps:

1. Add a Manual Trigger node
2. Add the Hacker News node
3. Configure the Hacker News node
4. Execute the node
5. Save the workflow

## Steps

### 1. Add a Manual Trigger Node
1. Open the nodes panel by selecting the `+` icon in the top right corner of the canvas or pressing `Tab` on your keyboard.
2. Search for the **Manual Trigger** node.
3. Select it when it appears in the search.
4. The Manual Trigger node is added to your canvas, allowing you to run the workflow anytime by selecting the **Test workflow** button.

**Note:** In real-world scenarios, you would likely use a scheduled trigger instead of a manual one.

### 2. Add the Hacker News Node
1. Select the `+` icon to the right of the Manual Trigger node to open the nodes panel.
2. Search for the **Hacker News** node.
3. Select it when it appears in the search.
4. In the **Actions** section, select **Get many items**.
5. The Hacker News node is added to your canvas, and its configuration window opens.

### 3. Configure the Hacker News Node
When a new node is added, it is automatically activated. Configure it as follows:

#### Parameters:
- **Resource:** All (retrieves all data records related to articles).
- **Operation:** Get Many (fetches all selected articles).
- **Limit:** 10 (retrieves up to 10 results).
- **Additional Fields:**
  - **Add Field > Keyword:** `automation` (filters results to only those with the keyword "automation").

  ![hackers news action node](https://github.com/user-attachments/assets/7150a8af-d57f-469c-86e2-0b5eb4939a15)


#### Settings:
- **Notes:** "Get the 10 latest articles."
- **Display note in flow?** Toggle to `true` (shows the note in the canvas).

![settings](https://github.com/user-attachments/assets/918e8e17-2fd1-4b93-b508-79e0b3707fc3)


### 4. Execute the Node
1. Select the **Test step** button in the node details window.
2. If configured correctly, 10 results should appear in the **Output Table** view.

#### Execution Details:
- A green checkmark on the node indicates a successful execution.
- Results can be viewed in **Table, JSON, or Schema** formats.
- Hover over the info icon next to **Output** to see:
  - **Start Time:** When execution began.
  - **Execution Time:** How long the node took to process data.
- If there are errors, a red warning icon will appear on the node.

### 5. Save the Workflow
1. Select **Back to canvas** to return to the main workflow.
2. Rename the workflow from "My workflow" to **"Hacker News Workflow"**.
3. Save the workflow using one of these methods:
   - Press `Ctrl + S` (Windows) or `Cmd + S` (Mac).
   - Select the **Save** button in the top right corner.

## Conclusion
By following these steps, you've successfully created a workflow to fetch and filter Hacker News articles about automation. You can extend this workflow by adding further processing steps or integrating with other services.

