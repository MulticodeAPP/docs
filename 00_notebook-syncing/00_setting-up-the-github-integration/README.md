https://multicode.app/n/docs/sync/file/setting-up-the-github-integration

# Setting up the GitHub Integration

1. Create a [new GitHub repository](https://github.com/new).
    - a public repository: public repositories are always supported, regardless of which subscription plan you are on (if any)
    - a private repository: you'll need a [Multicode Basic subscription](https://multicode.app/pricing) for private repository support

2. Create an export of your Multicode Notebook. (Notebook -> Settings -> Export Notebook). This will create a ZIP containing your notebook.

3. Connect your repository to your Multicode notebook. (Notebook -> Settings -> Connect to GitHub).

4. Extract the exported ZIP into the root of your newly created repository (without leading directories), commit and push this change.

5. Wait for Multicode to validate (and sync, if on your default/main branch) your notebook, and confirm it went successfully.
