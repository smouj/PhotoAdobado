# User docs: writing and review rules

These guides are part of PhotoAdobado. Write for someone trying to finish a photo task, not for a
developer. The source project is PhotoCraft; keep upstream names only when explaining upstream
history, technical identifiers, or a behavior that was actually reported there.

## Page rules

- Lead with the answer or next useful step.
- Use plain language, short paragraphs, and numbered steps for actions.
- Match menu and control labels to the current app.
- Link to related guides instead of copying them.
- Never present an upstream release, launcher, support channel, or feature as a PhotoAdobado release.
- Describe behaviors checked in the current PhotoAdobado source or a tested Adobado package. If a
  note comes from PhotoCraft, label it as upstream and say when PhotoAdobado has not been checked.
- Send PhotoAdobado bug reports to its [issue tracker](https://github.com/smouj/PhotoAdobado/issues).
  The [Adobado Kit website](https://smouj.github.io/Adobado_Kit/) links to the family of apps.
- Do not promise support through a community service unless the project publishes that channel.

## Frontmatter

    ---
    title: Export an image as PNG or JPEG
    description: One sentence for search results and link previews.
    order: 10                 # optional, sorts within the folder
    verified: 0.1.0-alpha.1   # only when checked against this PhotoAdobado release
    ---

Omit verified when there is no PhotoAdobado release or the page has not been checked against it.
Do not use a PhotoCraft version as PhotoAdobado's verified version.

## Before publishing

- Check links and UI labels.
- Confirm each product claim against current source or a tested package.
- Keep upstream issue and pull-request links only when they explain upstream provenance.
- Check the current README for the app's honest installation and test status.
