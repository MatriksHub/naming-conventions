# Pivotal Tracker Story Convention

### Pivotal Tracker Story Format

Based on the story type, different formats have been outlined.

### Feature Story

This should contain the following information

```
Title: (one line describing the story)
 
Narrative:
As a <type of user>  
I want <some goal> 
so that <some reason>
 
Acceptance Criteria: (presented as Scenarios)  

Scenario: Title  
Given <context>  
  And <some more context>...  
When  <event>  
Then  <outcome>  
  And <another outcome>...

Branch name  
Adhere to the branch naming convention for Workdey outlined in the wiki
```

#### Example:

```
Story Title: As a Taskee I should be able to grant the Tasker access for offline communication  

As a Taskee
I want to be able to make my contact information visible to the Tasker after successful completion of tasks
So that they can be able to contact me offline

Scenario 1:  
Given that I am a taskee 
And I have finished a task assigned to me 
And all payments have been completed,
When I log into dashboard, 
Then I should see a link where I can decide to share or decide not to share my contact info with the tasker

Scenario 2:  
Where necessary, the story should provide more scenarios that cover other edge cases.

Branch Name
ft-granting-offline-communication-123048761
```

**Note**: Every story title should include the word ‘should’ as opposed to ‘can’. e.g. It’s unclear whether the story “User can delete comment” is a feature or a bug. “User should be able to delete comment” or “User should not be able to delete comment” are much clearer: the former is a feature, the latter a bug.

### Bug Story

This should contain the following information:

```
Title  
A short description of the bug.

Description  
What is currently happening? What should be happening?

Instructions  
Outline the steps to reproduce/show the bug.

Resources  
Include screenshots and other assets to help explain/show the bug.

Branch name  
Adhere to the branch naming convention for Workdey outlined in the wiki.
```

#### Example:

```
Title: Unwanted spaces should not appear between tasks.

Issue
The number of tasks showing per row is inconsistent.

Expected  
When users view the pages containing the tasks, each row should contain 4 tasks per row. 

Instructions To Display Bug  
Search for tasks and scroll through the results.  
Some rows should display unwanted spaces in between the tasks.

Resources  
Attach a screenshot of the error caused by the bug if applicable.

Branch Name
fx-task-css-error-121944512
```

### Chore Story

This should include the following information

```
Title   
A short description of what needs to be done.

Description  
Why is it needed? Does it help the team go faster or is it a dependency that could cause problems in the codebase if it’s not done?

Resources  
Including instructions, additional context, or other assets that help execute the chore.

Acceptance Criteria
These should include conditions that must be met for the chore to be accepted.

Branch name(If applicable) 
Adhere to the branch naming convention for Workdey outlined in the wiki.
```

#### Example:

```
Title  
Add a Pivotal Tracker Story Convention page to the project wiki

Description
The wiki should serve as a comprehensive guide for anyone about to create a pivotal tracker story for the project

Resources  
1. https://www.pivotaltracker.com/blog/principles-of-effective-story-writing-the-pivotal-labs-way/
2. https://docs.google.com/document/d/1uh0q0ppRHP7PFwOjwb5JKJGIuKILjzZmubPAE1Yskb4/edit

Acceptance Criteria
1. A wiki page on Github that contains the comprehensive guide to creating Pivotal Tracker Stories
```

