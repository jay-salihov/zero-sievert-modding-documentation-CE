# SpeakerAddQuestion

### Syntax

`SpeakerAddQuestion(speaker_id, question_text, answer_text);`

**Returns** nothing.

| **Argument** | **Type** | **Description**                                      |
| :----------- | :------- | :--------------------------------------------------- |
| speaker_id   | String   | The ID of the speaker to modify.                     |
| question_text| String   | The text prompt that can be clicked on to provide an answer. |
| answer_text  | String   | The text shown when the prompt is clicked on.       |

This adds a new question and answer to the speaker's dialogue options.

### Example:

```
SpeakerCreate("test_npc") 
SpeakerAddQuestion("test_npc","What's your favorite kind of dog","A hot dog") 
```

This creates a speaker and then adds a question.