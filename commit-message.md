# Commit Message Convention

A commit message consists of a **header**, a **body** and a **footer**, separated by a blank line.

## Format of the commit message

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

Any line of the commit message cannot be longer than 100 characters! This allows the message to be easier to read on github as well as in various git tools.


### Message Header:

---

The message header is a single line that contains succinct description of the change containing a **type**, an optional **scope** and a **subject**.

`<type>`: This describes the kind of change that this commit is providing.

- feat (feature)
- fix (bug fix)
- docs (documentation)
- style (formatting, missing semi colons, …)
- refactor
- test (when adding missing tests)
- chore (maintain)

`<scope>`: Scope can be anything specifying place of the commit change. For example events, kafka, userModel, reviews, ratings, notification, dashboard, authorization, authentication, loginPage, etc...
This can be empty (eg. if the change is a global or difficult to assign to a single component), in which case the parentheses are omitted, i.e. scope is optional.

`<subject>`: This contains a very short and succinct description of the change.

- use imperative, present tense: “change” not “changed” nor “changes”
- don't capitalize first letter
- no dot (.) at the end


### Message Body

---

- just as in subject use imperative, present tense: “change” not “changed” nor “changes”
- includes motivation for the change and contrasts with previous behavior


### Message Footer

---

#### Referencing issues

Finished, fixed, delivered stories or closed bugs should be listed on a separate line in the footer prefixed with "Finishes", "Fixes" , "Delivers", or "Closes" keyword like this:

```
[(Finishes|Fixes|Delivers|Closes) #TRACKER_STORY_ID]
```

#### Example

```
Closes #234
```
or in case of multiple issues:
```
Closes #123, #245, #992
```


### Commit Message Example

---

```
feat(kafka): implement exactly once delivery

- ensure every event published to kafka is delivered exactly once
- implement error handling for failed delivery

[Delivers #130635935]
```

