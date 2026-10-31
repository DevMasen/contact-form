# Contact Form

This project is a single, unstyled HTML page that teaches how to build a real, accessible contact form. The page uses proper labels, grouped controls, and browser validation attributes — with no JavaScript and no CSS. Styling is left for a later project. The form posts to a placeholder URL so a server would receive the expected name and value pairs.

It follows the [Contact Form](https://roadmap.sh/projects/contact-form) exercise from [roadmap.sh frontend projects](https://roadmap.sh/frontend/projects/). Those projects walk through HTML, CSS, JavaScript, and full frontend builds from beginner to advanced. This page is the HTML contact-form step: structure the browser and the server actually rely on.

## How this was built

1. Read the project brief and the [roadmap.sh mockup](https://assets.roadmap.sh/guest/contact-form-hgkrw.png) for Acme Support (header, nav, fields, footer).
2. Created `index.html` with `<title>`, `<meta charset>`, and a viewport meta tag.
3. Laid out the page with a header, primary nav, main heading, intro copy, the form, and a footer.
4. Wired `<form action="https://example.com/contact" method="post">` so a submission would look like a real POST.
5. Added labeled controls paired with `for` and `id`:
   - Full name (`type="text"`, `required`)
   - Email (`type="email"`, `required`)
   - Subject (`<select>` with at least three topics plus “Choose a topic”)
   - Message (`<textarea>`, `required`, `minlength="20"`)
   - “How did you hear about us?” radios inside a `<fieldset>` with a `<legend>`
   - Optional “Send me product updates” checkbox
6. Added a `type="submit"` button labeled **Send message**.
7. Gave every control a `name` (and radios a shared name) so the request body is `full-name`, `email`, `subject`, `message`, `hear-about-us`, and `newsletter`.
8. Checked the page in the browser: labels, required/email/`minlength` validation, and the name/value pairs a backend would receive.

Open `index.html` in a browser to try native validation. There is still no backend; the action URL is a placeholder.

## Vote

Vote the project on this [link](https://roadmap.sh/projects/contact-form/solutions?u=66107474da1671f986289b45)

---

Built by [DevMasen](https://github.com/DevMasen).

Thank you for visiting this repository. If you are learning HTML forms too, I hope this page is a clear example of labels, grouping, and validation without extra tooling.
