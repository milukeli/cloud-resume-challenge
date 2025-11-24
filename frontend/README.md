# Frontend Technical Specification

- Create a static website that serves an HTML resume.


## Resume Format Considerations

I'm going to use [Harvard Resume Template format](https://careerservices.fas.harvard.edu/resources/bullet-point-resume-template/) as the basis of my resume. I'm in EU, and basically I used similar format for years now, never had any complaints.


### Harvard Resume Format Generation

I know basic HTML and CSS, but I'll let our friend ChatGPT do the heavy lifting and generate both HTML/CSS code and from there I'll modify it as needed.

Prompt to ChatGPT 5:
```text
Convert this resume format into HTML.
Please don't use a CSS framework.
Please use the least amount of CSS tags.
```

Image provided to LLM:
![](./docs/harvard-resume-format.JPG)

This is the [generated output](./docs/24-11-2025-resume-minimal.html) which I will tweak accordingly.

This is what the generated HTML page looks like unaltered:
![](./docs/resume-minimal-rendered.JPG)

## HTML adjustments
- UTF8 because it supports most known languages
- We will be applying mobile styling to our website so we'll include viewport meta tag width=device-width
- We'll extract styles into its own stylesheet once we're happy with our HTML markup
- We'll use indentation (2 spaces)