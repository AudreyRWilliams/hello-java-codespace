# "Hello World!" Java Program
The archetype generates a class `com.example.App` with a simple `"Hello World!"` <br>
<img width="280" height="319" alt="Screen Shot 2025-08-29 at 7 24 53 PM" src="https://github.com/user-attachments/assets/ee137669-61ca-4f70-a398-0c440dc431ad" />

<br><img width="633" height="61" alt="Screen Shot 2025-08-29 at 7 02 04 PM" src="https://github.com/user-attachments/assets/9fb912c9-2011-441b-a156-ea37b668cb30" />
## Here are the steps to recreate this project
## 1 — Create a new repo on GitHub

(Option A: web UI — easiest)

- Go to GitHub → <b>New repository</b> → name it e.g. `hello-java-codespace` → choose Public/Private → <b>Create repository</b> (leave it empty).
## 2 — Add the devcontainer files (directly on GitHub)

Create a folder called `.devcontainer` at the repo root with <b>two files:</b>
- .devcontainer/Dockerfile
- .devcontainer/devcontainer.json
<br>Why this approach? it’s explicit and reproducible: Codespaces will build the container, install OpenJDK 11 + Maven, and open VS Code in that container. (You can also let VS Code add prebuilt Java dev containers via the UI; both are supported.)
