PasswordInfringers
=============

Lists all sites that possibly store your password as plaintext, which you discover when signing-up or "forgetting" your password.

# Contributing

The sites, urls and additional notes are stored in `sites.json`. If you want to add a site to the list you'll need the following information:

- `name`: The name of the service.
- `url`: The url of the page.
- `status`: This is an indicator used on the site to determine the status of account deletion:
    - `easy`: Sites that previously stored the password as plaintext and appear to have updated.
    - `medium`: Responded to a contact saying they will work on improving it.
    - `hard`: Currently storing password as plaintext.
    - `impossible`: For sites where it's basically impossible to totally delete your account, even if you contact them
- `notes`: *(optional)* Notes will be shown when someone hovers on that service. Notes may include how you noticed that the password was stored as a plaintext (e.g. received e-mail upon creating an account).
- `email`: *(optional)* If you have to send an email to a company to cancel your account, add the email address here. We'll do the rest.

## Contribution checklist

1. Have you updated to the latest version of the project? `git pull`
2. If you have modified an existing service's status, please explain why/give sources.
3. URLs must be direct links to either deletion, or if this is not available, a relevant help article.
4. Any steps for the process should be detailed in the notes (if necessary).
5. Be sure to indent 4 spaces per level.
6. Be sure to place your entry ALPHABETICALLY in the current list.
7. Please test that your changes work validating `sites.json` with something like [JSON Lint](http://jsonlint.com/)

## Translation

If you want to translate the site:

1. Create a new `CODE.json` file in the `_trans/` directory where `CODE` is your [short country code](https://en.wikipedia.org/wiki/Country_code)
2. Copy the contents of `en.json` to your new file
3. Translate each line

### Style guide for Spanish Translations

Use guillemets (« ») for quoting statements that the website owner has published. Try to address the user as Tú instead of Usted. Write "haz clic" (hacer clic) instead of the verb "cliquear" or "clicar" because the former is the [RAE recommended way](http://lema.rae.es/dpd/srv/search?key=clic) of writing it.

## Misc

Search functionality modified from [DevCenter.me](https://github.com/stevestreza/DevCenter.me).

### Licence

This project is based on [justdelete.me](https://github.com/justdeleteme/justdelete.me).

Licensed under the MIT License (MIT).
Copyright (c) 2013 Robb Lewis, various contributors.
See `LICENSE.md`.

Country Flag Icons Copyright (c) 2013 Go Squared Ltd. http://www.gosquared.com/
