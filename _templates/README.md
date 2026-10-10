# Updating research highlights

Copy highlight-template.md into ../_highlights/ with a descriptive filename.
Edit its metadata and the three short Markdown sections.

section: "recent" places a project among recent works; section: "earlier" is for earlier works.
order sets the intended sequence within each section, lowest first.

Store optional figures in files/research/<project-slug>/ and use a path such as
/files/research/little-red-dots/figure.png in the image field. Fill in image_alt and image_caption.

The four entries are scientific drafts for author review.
The fast-X-ray draft uses Zheng & Lu's long-GRB cocoon paper, arXiv:2603.09674.

_config.yml registers the highlights collection with Jekyll. output: false means
individual highlights do not get standalone pages; a future shared layout will
assemble them into the research page.

The main page is generated at /research.html from research-review.md and _layouts/research.html.
Add a new project's slug to highlight_slugs in research-review.md to include it.
Earlier research remains available at /research-earlier.html.
The research-preview.md draft is excluded from publication.
