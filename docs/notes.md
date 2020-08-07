text came in well structured html, but in 7 parts.
split into chapters and cleaned up using refine.
exported as CSV.
used jekyll page gen to create markdown stubs.
then added stubs to project text

for f in *.html; do mv "$f" "${f%.html}.md"; done

word tree, http://linguistics.chrisculy.net/lx/software/DoubleTreeJS/
