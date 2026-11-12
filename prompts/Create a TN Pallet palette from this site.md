Create a TN Pallet importable colour palette from the website URL I provide.

First inspect the current https://github.com/cchatterton/tn-pallet repository. Read its README, JSON import implementation, validation rules, and relevant examples or tests. Establish the exact schema, naming constraints, section behaviour, and effect of importing on an existing palette. Treat the current code as the authority; do not assume a format from memory.

Then inspect the target site's sitemap, representative page types, stylesheets, CSS variables, and rendered elements. Include relevant responsive and interaction states where they affect colour use. Prioritise interface colours used for text, links, buttons, navigation, focus states, borders, cards, and section backgrounds. Exclude colours that appear only in photographs or illustrations.

Normalise the extracted colours by role. Use a SMACSS-inspired separation between foundational styles and theme variations, while fitting the sections supported by the current TN Pallet import format. Preserve actual source values and convert them to six-digit hex. Deduplicate identical values and record source aliases. Do not invent shades. Distinguish verified values from inferred roles, and explain any ambiguous classifications.

Produce:
- A JSON file ready for TN Pallet's JSON import.
- An HTML swatch preview showing each import identifier, hex value, original CSS variable or selector, and assigned role.

Validate the JSON with TN Pallet's actual parser or tests where practical. Otherwise, validate it against the current schema and say what could not be verified. Report the number of colours and sections, the main grouping decisions, and what importing will do to an existing palette.

Save both files as deliverables and link them in the response. Do not import the palette into WordPress.
