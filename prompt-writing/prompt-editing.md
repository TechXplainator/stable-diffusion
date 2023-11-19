# Prompt Editing

Prompt editing allows you to start sampling one picture, but in the middle swap to something else. 

## Start with Subject 1 and Change to Subject 2 at Step X

The base syntax is:

```markdown
[subject1:subject2:X]
```
X is a number indicating at which step to switch during the sampling cycle. The higher this number, the later the switch happens, and the model has less power to replace subject1 with subject2. 

**Example**: 

```markdown
a portrait of [Johnny Depp:Idris Elba:16]
``````
![Elba-Johnny](/images/prompt-editing/Elba-Depp.jpeg)

At start, the model will be drawing a portrait of Johnny Depp.
After step 16, it will switch to drawing a portrait of Idris Elba, continuing from where it stopped with Johnny Depp.

## Add Subject after X

The base syntax is:
```markdown
[subject:X]
```

**Example**: 

```markdown
fantasy landscape with a [mountain:lake:15]
``````
![mountain-lake](/images/prompt-editing/mountain-lake.jpeg)

At start, the model will be generating a fantasy landscape with a mountain. After step 15, it will switch to generating a fantasy landscape with a lake, but continuing where it stopped with the mountains. 

## Remove Subject at X

The base syntax is:
```markdown
[subject::X]
```

**Example**: 

```markdown
A bar [with red neon light::9]
``````
![bar](/images/prompt-editing/bar.png)

At first, Stable Diffusion will generate an image of a bar with red neon light. After 12 steps, it will switch to create an image of a bar, but based on the image of a bar with red neon light.


## Alternate Beteween Subjects
The base syntax is:
```markdown
[subject1|subject2]
```
**Example**: 

```markdown
A [pig|monkey] in a barn
``````
![pig-monkey](/images/prompt-editing/pig-monkey.png)

Stable Diffusion switches back and forth between creating an image of a pig in a barn and a monkey in a barn in each step.

You can expand this syntax to more than 2 subjects. In that case, Stable Diffusion will cycle through subjects 1, 2, up to N, and then loop back to subject 1:

```markdown
[subject1|subject2|...|subjectN] - alternates between subject1 ... subjectN, then loops back to subject1
```