+++
# Contact widget.
widget = "contact"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 160  # Order that this section will appear, after the gallery.

title = "Contact"
subtitle = "For partnership enquiries, tell me the objects, the data you hold, and the decision you need to make."

# Automatically link email and phone?
autolink = true

# Email form provider
#   0: Disable email form
#   1: Netlify (requires that the site is hosted by Netlify)
#   2: formspree.io
#
# Set to 0 deliberately. With a form enabled, the theme's contact widget hides the email
# address entirely (see themes/academia-hugo/layouts/partials/widgets/contact.html), and its
# Formspree integration posts to the legacy `https://formspree.io/<email>` endpoint, which
# Formspree retired in favour of per-form IDs (`https://formspree.io/f/<id>`). That combination
# gives visitors a form that silently fails and no address to fall back on.
#
# TODO: to restore a working form, either (a) create a Formspree form, then override the widget
# to post to `https://formspree.io/f/<your-id>`, or (b) if the site moves to Netlify hosting,
# set email_form = 1.
email_form = 0
+++

