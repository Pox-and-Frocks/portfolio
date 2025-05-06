# Research Site Template

[See the Demo Here](https://maxturer.github.io/research-site)

## A template for a single research project, adapted from [al-folio](https://alshedivat.github.io/al-folio/)

## Installing

1. Click on the "Use this template" button on the top right, and follow the instructions to create your own repository.
2. Go to https://github.com/settings/tokens and choose Generate New Token (classic is fine). Name it what you like (I used the same name as the repository I made in step 1), and copy the generated code (keep it pasted somewhere safe).
3. Back in your new repository, go to Settings --> Secrets and variables --> Actions, and create a new Repository Secret called LIGHTHOUSE_BADGER_TOKEN. Paste the code you just copied here as the "Value."
4. In your new repository, go to Settings --> Actions --> General, and make sure "Read and Write Permissions" is checked in the "Workflow Permissions" section. Check it if not, and save.
6. Next, go to Settings --> Pages. Choose "Deploy from a branch" as your build source (use your "main" or "master" branch for now).
5. Open the file _config.yml. Change the url from maxturer.github.io to [your username].github.io, and change the base url from /research-site/ to the name of your new repository (like: /new-repo-name/).
6. After a few minutes, head back to Settings --> Pages. The "deploy from a branch" dropdown should have a new branch available called "gh-pages." Choose this one instead, and save. If you don't see this branch yet, no worries, it can take up to 10 minutes to generate. It'll be there!
7. Wait (a while) for the action to run again, then you should have your site! Customize as you like.

## Further help

Check out the [al-folio readme and installation guide](https://github.com/alshedivat/al-folio) for more information.

## Presentation

If you're affiliated with GW, check out the [related presentation here](https://docs.google.com/presentation/d/1Gw3RLyDeMVuOPn7OlrnMHEVobKUDLkqXxGfVxUhRuYg). Thanks!

If you have any questions, send me an email at [max.turer@gwu.edu](mailto:max.turer@gwu.edu).