# "Hello World!" Java Program
The archetype generates a class `com.example.App` with a simple `"Hello World!"` <br>
<img width="280" height="319" alt="Screen Shot 2025-08-29 at 7 24 53 PM" src="https://github.com/user-attachments/assets/ee137669-61ca-4f70-a398-0c440dc431ad" />
<hr>
<br><img width="633" height="61" alt="Screen Shot 2025-08-29 at 7 02 04 PM" src="https://github.com/user-attachments/assets/9fb912c9-2011-441b-a156-ea37b668cb30" />
<hr>

## Here are the steps to recreate this project:
## 1 — Create a new repo on GitHub

(Option A: web UI — easiest)

- Go to GitHub → <b>New repository</b> → name it e.g. `hello-java-codespace` → choose Public/Private → <b>Create repository</b> (leave it empty).
## 2 — Add the devcontainer files (directly on GitHub)

Create a folder called `.devcontainer` at the repo root with <b>two files:</b>
- <b>.devcontainer/Dockerfile</b>
<img width="769" height="292" alt="Screen Shot 2025-08-29 at 8 24 12 PM" src="https://github.com/user-attachments/assets/1cab9a31-5c4e-4a4a-9613-123f80a562d2" /> <br>
- <b>.devcontainer/devcontainer.json</b>
<img width="445" height="349" alt="Screen Shot 2025-08-29 at 8 27 15 PM" src="https://github.com/user-attachments/assets/4cc38aa7-5847-4372-9224-1ffd31b7861d" />
<br><br>
Why this approach? it’s explicit and reproducible: Codespaces will build the container, install OpenJDK 11 + Maven, and open VS Code in that container. (You can also let VS Code add prebuilt Java dev containers via the UI; both are supported.)

## 3 — Create a Codespace for the repo

- On GitHub repo page → click <b>Code → Codespaces → Create codespace on main</b>.
- Wait for the Codespace to build the container. You’ll see a build log and once finished you’ll have a VS Code web/editor UI with a terminal. (See GitHub Codespaces docs for details.)

## 4 — In the Codespace terminal: generate a Maven project

Once the Codespace finishes building, open the terminal and run:

<img width="539" height="244" alt="Screen Shot 2025-08-29 at 8 35 27 PM" src="https://github.com/user-attachments/assets/fae5ac52-5c56-4d66-a8c5-86196833820b" />

This creates hello-java/ with src/main/java/com/example/App.java and test skeletons.

Build and run:

<img width="521" height="202" alt="Screen Shot 2025-08-29 at 8 40 54 PM" src="https://github.com/user-attachments/assets/f3a61813-88fd-4cec-b181-52d2745c0b0f" />

(If you prefer to hand-create a single `Main` class, create `src/main/java/.../App.java` and run the same `java -cp` ... command.)

## 5 — Commit the project and push to GitHub

<img width="395" height="118" alt="Screen Shot 2025-08-29 at 8 44 36 PM" src="https://github.com/user-attachments/assets/c83016d6-fedb-4e1c-93ea-086753de4adc" />

Now your repo contains both the `.devcontainer` and the Java project; anyone who opens the repo in a Codespace will get the same environment.
