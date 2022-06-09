# TexStudioMacros
A collection of macros for TeXStudio

# How to Install
1. Download the macros you want to install
2. Open TeXStudio
3. Got to `Macros -> Edit Macros...`
4. Click `Import`
5. Select the downloaded macro(s)

# Macro Descriptions

## gitInitAndSetupRemote
- Initialises a local repo
- Downloads GitHub's gitignore template for TeX projects
- Commits everything with a customisable initial commit message
- Asks to set up a GitHub remote, if yes:
	- Asks for the name, description and privacy
	- Pushes everything
	- :warning: Requires GitHub CLI to be installed and setup first, available here: cli.github.com

## gitPull
- Triggers to run on startup
- Checks the current doc is in a repo and has a remote to pull from
- Pulls if ok button clicked

## gitCommitAndPush
- Triggers to run upon finishing compile (may run more than once if doc takes multiple compiles to finish)
- Creates a dialog box for entering a commit message
	- Adds an option to push to remote only if one exists
- Commits and, if available and selected, pushes to remote