
Read through the relevant page fully before assuming something's broken,
most relevant issues are covered here. Still stuck? Visit the [Discord server](https://discord.gg/ZPaTpx82at) for assistance.

## Getting started

??? question "How hard would you say this is?"
    This is a glorified UTAU or DeepVocal if anything. You should at
    least understand the basics of creating a voicebank for either before
    picking this up; if you're not familiar with that already, you're likely
    to struggle.

??? question "What about CVVC and VCV?"
    Think of CVVC as a foundation to build on if you plan to include VCV.
    Standalone VCV is possible, but you'll need to pay close attention to how
    you optimize your transitions. It's up to you.

    ※ For example, the English "4/dx" phonetic may need VCV to work smoothly.

??? question "How does the pitch system function?"
    It's frequency-based, as a result, pitch suffixing doesn't matter. Be careful with
    your high range, as it can dominate your voicebank. For instance you should put 
	a falsetto in its own separate voicebank, or tag it with a special phoneme.

??? question "Should I clean my samples before labeling?"
    Not a bad idea at all. Do clean your samples before beginning work.

??? question "Are all these samples *seriously* necessary?"
    Generally, yes. On the other hand, optimization can go a long way.

## Building & porting

??? question "Should I work on this on an external drive?"
    Yes. Databases can come out to 1GB or 20GB+, in *dev* form. Do work on an
    external drive if you wish to, and believe it is appropriate to do.

??? question "I have a UTAU voicebank : can I port it ?"
    Possible, as long as it's not a CV bank. The result may come out slightly
    weird, though.

??? question "Can I create a Jinkiri-like voicebank, or use RVC?"
    Neither is encouraged.

??? question "Should I share my bank?"
    A mixed bag, as it's OK to distribute home-made databases, as long
    as you don't brand them as official, and you use discretion.

??? question "Why not just CV?"
    [Arsloid](https://vocaloid.fandom.com/wiki/ARSLOID_(VOCALOID4)#SOFT_).
    That's why. Jokes aside... The engine simply can't survive on CV alone. It's
    nowhere near as versatile as UTAU is for voicebank formats.

## Dictionaries & phonetics

??? question "Any advice on dictionaries?"
    Avoid the ones bundled with the devkit, they're known to have missing or
    wrongly-categorized phonemes. Use the dictionary collection linked in
    [Resources](resources.md) instead.

??? question "Why doesn't [-] work?"
    Make sure you have all your stationeries and openings set up. Beyond
    that, there's no obvious single cause.

??? question "What's up with the N\\ ?"
    Learn the context of the phonetic map for your desired language. In this case, `N\` is
    just one of several "N" phones for Japanese.

??? question "What's [?] ?"
    It is for glottal stops. Typically, they are categorized as "Glottal Plosives"
	in the dictionary.

??? question "What's up with the scales in the Editor ?"
    They're off by 1 — for example, C4 in a standard reference is C3 here.

??? question "How is a pseudo-EVEC created?"
    Add more vowels using the dictionary editor's **Special → Change Phonetic
    Unit Group**, then go from there.

## Errors

??? question "What do I do if the DB tool crashes?"
    Edits are saved in real time — just reopen it.

??? question "Voicebank compiler errors : what are -9 and -1?"
    `-9` is a segmentation error, usually an incomplete or incorrect
    configuration. `-1` is an audio format error.

??? question "What if the Dev Editor doesn't detect my bank?"
    Double-check both paths are correct, the only difference should be that
    one path ends in `.tree`. Keep voicebank names short and simple: no
    periods, instead use underscores.

??? question "What if my CompIDs overlap?"
    Make another one — preferably one you wrote yourself rather than an
    auto-generated one.

??? question "How do I make XSY presets (or presets in general)?"
    Use the Singer Editor to export them, then add them to your bank when you
    release it.

## Usage in other Editors

??? question "What about usage in other Editors ?"
    Piapro Studio, Tunelab, and V3-6 will all work.
    Setup workflow may differ slightly between them.
