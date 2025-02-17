#  Assistant System Prompt Generation .... System Prompts!

[![Part of AI-Assistants Library](https://img.shields.io/badge/Part%20of-AI--Assistants%20Library-blue)](https://github.com/danielrosehill/AI-Assistants)

![alt text](banner.jpg)

17-Feb-25

## Table of Contents - Assistant Configurations

This repository contains several assistant configurations for different purposes:

- [Multi-Purpose Configuration](multi-purpose.md) - A versatile configuration for system prompt generation
- [Parameter Tuning Assistant](tuner.md) - Specialized for fine-tuning model parameters
- [General Editor Configuration](editors/general-editor.md) - For general system prompt editing
- [Voice Editor Configuration](editors/editor-for-voice.md) - Specialized for voice assistant prompts
- [Markdown Generator Configuration](generators/generate-to-md.md) - For generating markdown documentation

## Temperature And Parameter Settings

Creating effective AI assistance for the purpose of drafting system prompts for other AI assistants Is a tough balancing act which requires a mixture of faithful adherence to the system prompt as well as some creativity in coming up with effective configurations and embellishing upon the user's ideas where that is asked for in the prompt.

Therefore pinning down the perfect temperature setting is especially hard. A more deterministic setting is helpful where prompt adherence is challenging but comes at the price of diminished creatiivty. 0.5 is about where I find best success.

## One "Meta" Assistant Or Many Task-Specific Ones

I've had good success with an elaborate configuration that instructs the assistant to:

- Improve upon the system prompt I've drafted.   
- Generate a two line description in the appropriate person.   
- Come up with a few alternative name suggestions.   
- Recommend a temperature for the configuration and other parameters.   
- Recommend a good underlying model to use.   
- Come up with a couple of good ideas for avatars
- Provide an actual text to image prompt for one of them. 

This took some careful prompt writing to achieve, however. 

So at the time of writing, I can see that it's definitely possible to chain a workflow together in one system prompt. Although as many things in prompt writing, you might find that it's best to chunk the task by reducing the purview of each agent to just one part of the process.

## "Don't Follow The Prompt!"

If you are using this system prompt generation approach, you might find it highly worthwhile to have a prompt available at a shortcut which corrects a model that has gone off-course in completing the task. 

One challenge you will encounter in asking AI agents to generate system prompts for other AI agents (or anything that is similarly a bit 'meta') is that sometimes they will follow the draft system prompt themselves rather than edit it (ie, they take it as an instruction!). I've had this happen many times but all it usually takes is "No, your task is to follow YOUR system prompt and edit this one" quickly gets things back on course. 

More proactive mitigation strategies, however, include:

- Using a very instructional model.   
- Minimal temperature setting where possible. 
 

## Author

Daniel Rosehill  
(public at danielrosehill dot com)

## Licensing

This repository is licensed under CC-BY-4.0 (Attribution 4.0 International) 
[License](https://creativecommons.org/licenses/by/4.0/)

### Summary of the License
The Creative Commons Attribution 4.0 International (CC BY 4.0) license allows others to:
- **Share**: Copy and redistribute the material in any medium or format.
- **Adapt**: Remix, transform, and build upon the material for any purpose, even commercially.

The licensor cannot revoke these freedoms as long as you follow the license terms.

#### License Terms
- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **No additional restrictions**: You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

For the full legal code, please visit the [Creative Commons website](https://creativecommons.org/licenses/by/4.0/legalcode).