# Gym Plan project notes

Static workout tracker (`index.html`, served by GitHub Pages from `main`). Each training day is an entry in the `DAYS` list at the top of the script.

## Exercise demo videos

When asked to find, add, or replace YouTube videos for an exercise:

1. **Search DeltaBolic first.** Channel: Andrew Kwong (DeltaBolic), https://www.youtube.com/@DeltaBolic/shorts. His Shorts are the preferred source. Search with the channel name plus the exercise, for example `DeltaBolic shorts leg extension`, and look for his titles ("The PERFECT ...", "Do ... LIKE THIS!"). Use a video only if it is the exact exercise.
2. **If DeltaBolic has no matching video**, find another short YouTube video (a Short, or the shortest clear form demo) for that exercise.
3. Use the video ID from the URL (`youtube.com/shorts/<ID>`). YouTube cannot be opened from the cloud sandbox, so channel credit and playback cannot be checked there. Tell the user the videos are unverified and ask them to play each once.
4. Videos the user has said work should not be replaced unless asked.

## Workflow

Make changes on the designated branch, then open a pull request into `main` and merge it, because GitHub Pages builds from `main`.

## Drop set definition (keep every day consistent)

The page defines a drop set once (`DROP_SET_RULE`, `DROP_HINT_PIN`, `DROP_HINT_DB` at the top of the script). Reuse those constants for any new day instead of writing new wording:

- A drop set is how you finish the last set, not an extra set.
- Start the last set with the same heavy weight as the set before and rep to failure.
- With no rest, lower the weight by about 20 to 30% (dumbbells about 2 steps, machine pin 2 to 3 plates) and rep to failure again, then drop once more and go to failure a third time.
- The "Drop-set weight" box holds the first drop weight.
