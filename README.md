# Feedback App

An app for collecting feedback on Markdown files. All feedback is stored in the
Markdown files themselves, in a format suitable for viewing in plaintext and
compatible with other Markdown renderers.

## Planned Architecture

The Markdown file is a literal file on the server. In the long term we may
support getting the file via an OAuth integration, principally with Github.

The server is responsible for A) parsing the Markdown file and B) saving updates
from the frontend. The frontend shouldn't be concerned with the underlying form
in which the data is stored.
