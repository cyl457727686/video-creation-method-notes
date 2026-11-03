# Video Creation Method Notes

[简体中文](README.md) · [English](README_EN.md)

**MiniMax H3 · Seedance 2.5 · Seedance 2.0**

Case-based methods for storyboarding, video prompts, animation and output review. The notes turn broad requests such as “natural motion” into observable actions, camera paths, spatial relationships and sound events.

**Package: V006 · Research notes: V005 · Updated: 2026-11-03**

## Install the skill

The portable `video-creation-methods` skill selects the appropriate model reference. Use an AI assistant that supports Agent Skills; ordinary chat products may instead require uploading the relevant Markdown file.

With [Node.js](https://nodejs.org/) 22.20 or newer, run this in your project:

```bash
npx skills add cyl457727686/video-creation-method-notes --skill video-creation-methods
```

Choose your assistant when prompted. This command uses the third-party [Vercel Skills CLI](https://github.com/vercel-labs/skills). Alternatively, download the Skill ZIP from the latest GitHub Release and place the complete `video-creation-methods` directory in your assistant's supported skills location. Keep its reference files and reload the assistant as required.

For assistants supporting `$skill-name`, try:

```text
$video-creation-methods
I am using Seedance 2.0 for an animated shot: [story beat].
References: [attach or describe]. Dialogue: [exact original words].
Review the action, space, camera and sound, then write a prompt for this model.
Respond in English and preserve the original dialogue language.
```

Other assistants use their own skill menu or invocation syntax. The skill entry is in English; detailed research references are currently in Chinese. A multilingual assistant can use them and respond in English. There is no full English translation of the three guides yet.

The skill supplies creative guidance, not a generation backend. It contains no executable scripts, API keys or automatic paid-generation calls.

## Choose a model guide

| Model | Guide | Focus |
| --- | --- | --- |
| MiniMax H3 | [H3 guide](H3学习增强版_V005.md) | Base modes versus Ref2VA, reference roles, visible events and audio fields |
| Seedance 2.5 / Jimeng | [2.5 guide](即梦Seedance2.5学习增强版_V005.md) | Material roles, event order, sound, and API-versus-product boundaries |
| Seedance 2.0 / Jimeng | [2.0 guide](即梦Seedance2.0学习增强版_V005.md) | Its own reference and task conventions, without importing 2.5-only parameters |

Select the guide for the actual model rather than loading all three for every task. You can also upload that Markdown file directly to an AI assistant, provide your scene, assets and dialogue, and ask it to apply the relevant methods using the model's current official format.

## What the methods cover

- Reference conflicts: separate identity, scene layout, state, style and voice responsibilities.
- Readable action: establish an initial state, necessary contact or force, and visible consequences.
- Camera design: describe starting composition, movement path, landing and storytelling purpose separately from character motion.
- Animation: organize value and edge hierarchy, spatial layers, key poses and primary versus secondary motion. Matte rendering, fog and particular frame cadences remain optional style choices.
- Sound: distinguish speakers, listeners, synchronous events, ambience and audience-only score.
- Diagnosis: separate source inputs, prompts, generated clips, editing choices and final results.

## Learning materials and original sources

| Case | Materials studied | Main lessons | Original sources |
| --- | --- | --- | --- |
| **First Date — Loop Forge** | Final film, making-of tutorial, 21 generation prompts, shared reference images and raw clips, music list and DaVinci Resolve project | Reference roles, hand contact, reactions and generation-versus-editing decisions | [Project and prompts](https://loopforge.cc/projects/h3-first-date/) · [Making-of](https://www.youtube.com/watch?v=fQ8HZC_dTXs) · [Author's assets/project](https://loopforge0.gumroad.com/l/firstdate) |
| **Loop Forge H3 camera tutorials** | Both tutorials, demonstrations, public prompts and explanations, and the repository's post-production speed script | Camera paths, subject motion, observed failures and speed changes after generation | [Case index](https://loopforge.cc/projects/h3-camera-shots/) · [Part 1](https://www.youtube.com/watch?v=GCdKh_KaQVs) · [Part 2](https://www.youtube.com/watch?v=28XEpsdJqVQ) · [Author repository](https://github.com/loopforge0/minimaxh3-shots-skills) |
| **ONEIRIC** | Public final film, production account and two explicitly paired prompt/generated-clip examples | Multi-character space, performance objectives, action causality and narrative transitions | [Public project](https://higgsfield.ai/@higgsfield.studio/projects/oneiric) |
| **RED FLAG** | Public final film, project description and author's production retrospective | Prop states, contact, direction, scene states, cuts and sound layers | [Public project](https://higgsfield.ai/@higgsfield.studio/projects/red-flag) |
| **KÖK BÖRÜ** | Public final film, project description and displayed design materials | Animation readability, spatial layering, key poses, motion hierarchy and state handoffs | [Public project](https://higgsfield.ai/@higgsfield.studio/projects/kok-boru-film) |

The camera case contains two tutorials. First Date includes a roughly one-minute final film and a separate making-of video. Only First Date and the camera tutorials are treated here as H3 cases; the other films are not collectively attributed to H3 or any one model. A complete shot-by-shot prompt → generation → final-edit chain was not obtained for the other three films.

Study used player images, extracted frames and reduced contact sheets, plus machine-assisted analysis of actual audio. Studying a source does not certify every detail. Source links may require login or author-provided download steps; this repository does not redistribute their media or projects.

## Evidence and maturity

These are research methods, not model training, fine-tuning or an official certification. Installing the skill improves access to the notes; it does not establish that they improve model outputs.

There is no controlled target-model comparison or guaranteed success rate. Some visual observation was delegated with key evidence reviewed by the primary agent. Audio was processed with speech recognition and audio-understanding models, with known errors corrected; this is not direct continuous listening or full lip-sync certification. The internal observation records and raw analysis are not included, so the public package cannot independently reproduce every coverage claim.

The references retain clearly marked conventions from the original project. Its English Seedance descriptions, asset approval records and independent TTS choice are not universal model requirements. H3's official language and syntax rules remain model-specific. Jimeng account controls must be checked in the real interface; API documentation alone does not establish UI capabilities.

Further details: [sources and verification](SOURCES.md) and [evidence limits](LIMITS.md), currently in Chinese. Official entry points: [H3](https://github.com/MiniMax-AI/MiniMax-H3/blob/main/.claude/skills/h3-prompt-writing/SKILL.md), [Seedance 2.5](https://docs.volcengine.com/docs/ark/seedance-2-5-prompt-guide?lang=zh), [Seedance 2.0](https://docs.volcengine.com/docs/ark/seedance-2-0-prompt-guide?lang=zh).

## Feedback

Open an Issue with the affected guide/section, model and product entry point, intended behavior, actual output, and a minimal example you can share. Distinguish a formatting problem from a method that does not fit the shot or a model that did not follow the request. Do not include secrets, private URLs or material you cannot publish.

## License status

No reuse license has been selected yet. This package does not grant rights to third-party films, prompts, assets or official documentation. Public availability is not represented as permission to redistribute source material.

[Changelog](CHANGELOG.md) · [Sources](SOURCES.md) · [Limits](LIMITS.md)
