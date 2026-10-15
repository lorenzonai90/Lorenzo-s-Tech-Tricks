# Lorenzo’s Tech Tricks

A responsive, static website built with HTML, CSS, and JavaScript.

## Files
- `index.html` — complete website, styles, theme settings, service cards, contact links, and booking form.

## Important: activate booking email delivery
The booking form uses FormSubmit's AJAX endpoint and sends requests to `lorenzonai90@gmail.com`. FormSubmit requires the inbox owner to activate the destination email the first time:
1. Deploy the site or open it from a local web server.
2. Submit a test booking with non-sensitive test details.
3. Check `lorenzonai90@gmail.com` for FormSubmit's activation/confirmation email and approve it.
4. Submit another test request and verify the received email subject matches the selected help topic.

Email delivery cannot be verified or activated from this generated package. Until activation is completed, do not advertise the booking form as fully live. The site shows an error if the submission service rejects the request and never claims an appointment is confirmed.

## Publish with Cloudflare Pages
1. Create a Cloudflare account and open Workers & Pages.
2. Create a Pages project and upload the folder contents (or connect a Git repository).
3. No build command is required for this static site. Set the output directory to the folder containing `index.html`.
4. Open the published URL on a phone and computer, test contact links, themes, and a booking request.

GitHub Pages also works: upload `index.html` to a repository and enable Pages in repository settings.

## Notes
- The theme preference is stored in local browser storage when available.
- The contact number and email are configured as supplied.
- Do not ask customers to provide passwords, payment information, or sensitive account credentials in the booking form.
- A booking request is not an appointment confirmation.
