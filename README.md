# A Resume Built in Latex

I've been writing my resume in LaTeX for a while using a template that I've customized, so I figured I'd put in on GitHub for others to see an example of a LaTeX resume.

Each resume section is in its own input file which are all included via LaTeX commands like `\input{education.tex}`.

The pdf may be out of date with the LaTeX content as I have to build then commit and push every time I update content, but I'll try to keep it updated with what the template looks like in pdf form.

# Custom LaTeX commands
I've wrapped some common formatting into LaTeX commands, which are documented below.

## Section Headings
`\SectionHeading{Education}` produces the headings for each section in my resume and sets a `0.25em` vertical spacing after the heading. It also typesets the headings in a small uppercase font. This is achieved through this LaTeX code:

```
\newcommand{\SectionHeading}[1]{\spacedlowsmallcaps{#1}\vspace{0.25em}}
```
