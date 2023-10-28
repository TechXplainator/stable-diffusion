# Prompt Formula for Stable Diffusion

Stable Diffusion is a software that uses AI to create images. To guide it to create the image you want, you can use positive and negative prompts. Positive prompts are words or phrases that tell the software what you want to see in the image, while negative prompts tell it what to avoid. 

Creating a good prompt is crucial. In fact, there are numerous websites where people seek ways to improve their prompt writing skills. This interest has given rise to a term called "prompt engineering.”

For the best results in generating images, a good prompt needs to include specific elements out of certain categories.

## Subject

The subject is what you want to see in the generated image. Ask yourself: do I want an image of a person? An animal or perhaps a landscape? 

For instance, let's focus on "a cat" as our subject.

Then, we need to consider the following questions:
- How do you characterize the cat? For instance, is the cat "adorable"?
- Are there particular characteristics you want for the cat? For example, the cat has "black fur and blue eyes."
- Where can the cat be found? For instance, "the cat is resting on a table."
- Are there any additional items the cat should have? For example, the cat is "wearing a red collar."

These questions collectively result in the following prompt formula:

```markdown
<Adjective> Subject <Action or Accessory> <Location>
```

- **Subject**: This is the central element you're addressing or emphasizing in your description. The subject can encompass a wide range of things, such as people, animals, objects, locations, plants, vehicles, food, weather conditions, natural occurrences, and abstract ideas.  It's the only mandatory part of the formula, so you must include it.
- **Adjective (Optional)**: You can use an adjective to add a descriptive word that helps paint a clearer picture of the subject. Adjectives can come before or after the Subject. This means you can use descriptive words to talk about the Subject, and you have the flexibility to place them before or after the main focus of your image.
- **Action or Accessory (Optional)**: This is where you can include an action or an item that's related to the subject, but it's not required.
- **Location (Optional)**: If you want to specify where the scene takes place, you can use this element. However, it's also optional.

In this formula:

- All the elements enclosed in angle brackets <...> are optional. This means you can choose whether or not to include them in your prompt.
- The only mandatory element is the Subject, so you must include it to describe the main focus of your image.
- The order of elements is not fixed, allowing you to place Adjectives, Actions or Accessories, and Locations before or after the Subject. This flexibility lets you craft your prompt in a way that best suits the context or your creative vision.

## Examples

### A Cute Black Cat

```markdown
A cute black cat with blue eyes wearing a red collar lying on a table
```

- **Subject:** cat
- **Adjective:** cute, black, with blue eyes
- **Location:** lying on a table
- **Action or Accessory:** wearing a red collar

### A Cheerful Yound Woman in a Garden

```markdown
a cheerful young woman with long, curly hair holding a bouquet of colorful flowers in a garden
```
- **Subject:** woman
- **Adjective:** cheerful, young, with long curly hair
- **Location:** in a garden
- **Action or Accessory:** holding a bouquet of colorful flowers

### Enchanted forest with ancient trees

```markdown
Enchanted forest with ancient trees.
```

- **Subject:** Forest
- **Adjective:** Enchanted
- **Location:** Not specified
- **Action or Accessory:** Ancient trees

### A curious cat exploring a mysterious cardboard box

```markdown
A curious cat exploring a mysterious cardboard box.
```

- **Subject:** Cat
- **Adjective:** Curious
- **Location:** Not specified
- **Action or Accessory:** Exploring a mysterious cardboard box

### Delicious pizza at a cozy Italian restaurant

```markdown
Delicious pizza at a cozy Italian restaurant.
```

- **Subject:** Pizza
- **Adjective:** Delicious
- **Location:** Cozy Italian restaurant
- **Action or Accessory:** Not specified

### Sparkling stars in the dark night sky

```markdown
Sparkling stars in the dark night sky.
```

- **Subject:** Stars
- **Adjective:** Sparkling
- **Location:** Dark night sky
- **Action or Accessory:** Not specified

### Tranquil waves lapping the sandy beach

```markdown
Tranquil waves lapping the sandy beach.
```

- **Subject:** Waves
- **Adjective:** Tranquil
- **Location:** Not specified
- **Action or Accessory:** Lapping the sandy beach

### Joyful children playing with colorful balloons in the park

```markdown
Joyful children playing with colorful balloons in the park.
```

- **Subject:** Children
- **Adjective:** Joyful
- **Location:** Park
- **Action or Accessory:** Playing with colorful balloons

### Racing down the winding mountain road, a sleek sports car

```markdown
Racing down the winding mountain road, a sleek sports car.
```

- **Subject:** Sports car
- **Adjective:** Sleek
- **Location:** Not specified
- **Action or Accessory:** Racing down the winding mountain road

### Wise old owl perched on a moss-covered branch

```markdown
Wise old owl perched on a moss-covered branch.
```

- **Subject:** Owl
- **Adjective:** Wise
- **Location:** Not specified
- **Action or Accessory:** Perched on a moss-covered branch

### The power of love connecting people across the world

```markdown
The power of love connecting people across the world.
```

- **Subject:** Power of love
- **Adjective:** Not specified
- **Location:** Not specified
- **Action or Accessory:** Connecting people across the world

### Busy city street, filled with rushing commuters

```markdown
Busy city street, filled with rushing commuters.
```
- **Subject:** City street
- **Adjective:** Busy
- **Location:** Not specified
- **Action or Accessory:** Filled with rushing commuters
