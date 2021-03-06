# backstage-test

## Steps
1. Generate devcontainer files.
    CMD + Shift + P to open command palette.
    Select `Codespaces: Add Development Container Configuration Files...`.
    Select Node latest, add Docker-in-docker support.

2. Create Backstage App
    ```bash
    npx @backstage/create-app
    ```

    Answer CLI options. 
    SQLite

3. Run the App
    ```bash
    cd my-backstage-app
    yarn dev
    ```

    The yarn dev command will run both the frontend and backend as separate processes (named [0] and [1]) in the same window. When the command finishes running, it should open up a browser window displaying your app. If not, you can open a browser and directly navigate to the frontend at http://localhost:3000.

    To start frontend and backend seperately, run these commands in seperate terminals:
    ```bash
    yarn start
    yarn start-backend
    ```