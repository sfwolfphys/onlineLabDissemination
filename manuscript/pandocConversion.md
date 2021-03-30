## To convert from LaTeX to Word with mostly good formatting

pandoc onlineLabPaper.tex --bibliography=onlinelabs.bib --filter pandoc-citeproc --csl american-physics-society.csl -M reference-section-title=References -o onlineLabPaper.docx

### Citation styles
Other citation styles exist (obviously). I downloaded this csl file from [citationstyles.org](https://citationstyles.org).

### Issues:

- ***Acknowledgements*** section title is missing. Not sure how to fix. I don't have the desire to look more than I have (5 minutes)
- Also ***Section numbering*** is broken.  I guess I'm putting those in manually too. (This can be done in MS Word/Libre Office by editing the style of `Heading 1` and `Heading 2`.  I can't make them align like I want them to (flush with the left margin), but whatever.
- There is a ***weird sticky space*** (yes, that's my technical term) that shows up right before citation brackets.  I did a global find-replace to get rid of them.

I've been told that they can "work with" anything I give them in Word. So we are going to test that a bit.
