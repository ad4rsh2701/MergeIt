## MergeIt

Just Another Stupid PDF Merger (JASPM? Potential new name?), for Windows.

I just don't feel like opening websites to merge my PDFs anymore, nor do I have the patience to keep updating `PATH_TO_PDF` variable
in my python script, hence we have this abomination.

*MISSING: Add build steps, how to's, etc. It's still just on paper, let me implement it!*

What to expect:
- Select multiple PDFs, right click and convert them to one single PDF
- Select one or multiple images, right click and convert them to one single PDF
- Select multiple images and PDFs, right click and convert them to one single PDF (maybe? I don't have this on paper)
- Select one or multiple docs, right click and convert them to one single PDF (I don't do this often, but good scope creep)


> I will be using `winreg` for messing with Windows Registry.
> And look, I can't seem to find *any* good resource on "PDF merging", I did get *some* resources on PDF structure, its objects and "tree".
> Though, I *still don't get how things are inside a PDF*, but I do have a high level overview. That won't make me write code in Rust though, so I will
use the following dependencies:
> 1. `lopdf`: For merging PDFs
> 2. `krilla`: For creating PDFs (e.g. Image to PDF)
