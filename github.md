# Github - How To

This document attempts to provide details on how to successfully contribute to open-source projects.  As such, it may be broken down into separate documents in the future depending on how it evolves (based on feedback).

## Easiest Way to Contribute.

The simples way to contribute to open source are the things that are needed that have nothing to do with the "source" such as:

- Leverage the project and if you encounter problems...
- Report Issues.
- Engage in Discussions (if enabled)... if not, utilize Issues to start conversation.
- If a project doesn't currently have *CI*, assist.
- If a project doesn't currently deploy as a *nuget* package, assist.
- Documentation, documentation, documentation!

The number one thing to keep in mind regarding all of the above is that the answer to your suggestions, issues, and/or contributions may be met with a "No".  Try not to take it negatively; remember that there may be plans in place that they are already engaged in that may either duplicate or invalidate your contribution.  Which takes me to the second "rule" to keep in mind... engage positively in all of your interactions - no one, including yourself, want to interact with those that start off a conversation negatively.  Remember... flies... honey... vinegar.

## Create a Successful Issue.

(TODO)

## Contribute Code.

There are several things that you'll need before you can contribute code to a repo.

- Assume a project is utilizing the latest version of Visual Studio unless they've made mention otherwise.
- You'll need *git* installed on your machine.
- You'll need a GitHub.com account.

With the *tools* out of the way, some things to consider before attempting to contribute to the source.

Start with creating/comment on an issue.  In general, when first visiting a repo, it's not a bad idea to first comment on an issue (if one exists) or open an issue on the topic.  Mention that you're interested in contributing and ask if that's OK.  Doing so let's the team (and others) know that you are considering tackling a particular subject and if there are things that you need to know about regarding contributing, the team can be sure to loop you in.

Also some repos have a general rules in places that new features (*pull requests*) are immediately closed (not reviewed) unless explicit permission was given out to someone to work on it.

In many repos, there are generally *issues* that have been flagged as being "up for grabs".  You can comment on these letting everyone know that you are considering contributing to those.

Once you submit the *pull request*, be sure to keep current with it so that if any request for changes or other feedback is provided that you can respond to them in a timely manner.  Doing so can increase the likely-hood of getting the request accepted.

As a side note, if you are familiar with anyone on the team and they asked you to specifically "break a rule", be sure to *tag* them in the *pull request*.

It is also important keep in mind that "just because you did the work" doesn't mean that your work will be accepted; this is normal and please respect it.

### Fork

It is not possible (unless you are on the primary team) to contribute code directly to someone elses repo.  To get started, you'll need to *fork* their project into your account.

(TODO: Walkthrough)

### Branch

Although not absolutely necessary, it kind of makes sense to create a developmental branch for your changes.  By doing this, you can keep the main branch up to date with the source repo (see below) and keep your code separate.  It is also recommended that you make your branches such that your code changes are as small as possible so that they can be more easily accepted (see below).

**Using GitHub Desktop**

- Verify that you have the correct repo (yours) selected for the *Current repository* dropdown.
- Click on the *Current branch* dropdown to display more details.
- Click the *New branch* button.
- In the *Create a branch* dialog, enter a meaningful name for the branch.
- Click *Create branch*.
- You will then want to *publish* the branch to your repo.

**Using Git (CLI)**

(TODO)

### "Atomic"

When making a contribution, make it **small**.  Sure, sometimes this isn't possible... however, you should always go into each contribution with this mindset.  Don't make the specific change that you desire to contribute along with several other, possibly meaningless, but certainly unrelated changes.  Focus, focus, focus.

(TODO: Example of both wrong and right ways)

### Pull Request

Once you are ready to submit your contribution, you do this through a *pull request*.  This is where you create a package of your changes to push to the original repo a form that they can review and then pull into their codebase.

(TODO: Walkthrough)

### Pull Request - Changes

It is possible that the target repo team may like what you've done and are very close to accepting the *pull request* but would like to see a few changes.

(TODO: Walkthrough / Example)

### Pull Request - Cancel

The *pull request* was completely rejected so there's really might not be any point in keeping it around in your repo, so how do you get rid of it?

(TODO: Walkthrough)

### Pull Request - Accepted

Now that the *pull request* was accepted and merged into the upstream repo, what do you do on your *fork* to keep things clean?

(TODO: Walkthrough)

### Keep Updated

It's been a while since you *forked* the upstream repo and they've made a lot of improvements since you've done so.  How do you keep things *cleanly* up-to-date witht he upstream repo?

Although Github.com has some mechanisms to assist with this, it creates additional *commits* that add "noise" to your repo.  It's simply confusing to see:

> This branch is 3 commits ahead. 50 commits behind.

When the only reason why it's "3 commits ahead" is that you utilized Github.com to merge (via *pull request*) the upstream changes into yours.

I submit that it would make more sense to cleanly "refresh" your main repo to *match* the upstream.  To do so...

```
   git fetch --all
   git checkout your_branch
   git reset --hard upstream/their_branch
```

Where *your_branch* is the branch that is in your repo that you want to "bring up to date* to match *their_branch* in the original repo.
