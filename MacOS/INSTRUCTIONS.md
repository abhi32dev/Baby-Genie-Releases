# Baby Genie — Quick Start & Setup Guide ✨
Your personal intelligent companion in the macOS menu bar.

====================================================================
TABLE OF CONTENTS
1. Installation (Drag & Drop)
2. Opening for the First Time on macOS (Security Prompt)
3. Connecting an AI Engine (Claude or OpenAI / Codex)
4. Making Your First Wish
5. Troubleshooting & Common Questions
====================================================================

--------------------------------------------------------------------
1. INSTALLATION
--------------------------------------------------------------------
1. In the installer window, drag the "Baby Genie" lamp icon directly 
   into the "Applications" folder shortcut.
2. Open your "Applications" folder and double-click "Baby Genie".


--------------------------------------------------------------------
2. OPENING FOR THE FIRST TIME ON MACOS
--------------------------------------------------------------------
Because Baby Genie is an independent app downloaded from the web 
(and not through the Mac App Store), macOS Gatekeeper displays a 
security notice the very first time you launch it.

Here are the 2 quick ways to approve it:

METHOD A: Via System Settings (Recommended for everyone)
1. If macOS shows a popup saying Apple cannot verify it, click "Done" or "OK".
2. Open your Mac's "System Settings" from the Apple menu ().
3. Click "Privacy & Security" in the left sidebar and scroll down to "Security".
4. You will see a message: "Baby Genie was blocked to protect your Mac".
5. Click the "Open Anyway" button next to it.
6. Enter your Mac password or Touch ID, then click "Open".
(Note: You only ever have to do this once. After this, it opens normally forever!)

METHOD B: Fast 1-Second Terminal Shortcut (For power users)
If you prefer, open Terminal and paste this one line:

xattr -cr "/Applications/Baby Genie.app"

Press Enter, and then double-click "Baby Genie" in Applications. 
It will open immediately with zero security prompts.


--------------------------------------------------------------------
3. CONNECTING AN AI ENGINE (Claude or OpenAI / Codex)
--------------------------------------------------------------------
Baby Genie works by using an AI assistant on your Mac to build and 
update your widgets whenever you make a wish. It supports both 
Anthropic (Claude) and OpenAI (Codex).

Pick whichever AI you prefer to power your Genie:

--- OPTION 1: Using Claude (Recommended) ---
1. Open Terminal (press Cmd + Space, type "Terminal", press Enter).
2. Install the Claude tool by pasting this command:

npm install -g @anthropic-ai/claude-code

3. Once installed, log in by typing:

claude

4. Press Enter. It will open your web browser to sign in to your Claude account.
Once signed in, Baby Genie is immediately connected!


--- OPTION 2: Using OpenAI / Codex ---
1. Open Terminal.
2. Install the Codex CLI tool by pasting this command:

npm install -g @openai/codex

3. Log in by typing:

codex login

Follow the prompt to connect your OpenAI account.


(Prerequisite Note: Both tools use Node.js. If your Mac says "npm: command not found", 
simply download the free installer from https://nodejs.org, install it once, 
and run the command above.)


--------------------------------------------------------------------
4. MAKING YOUR FIRST WISH
--------------------------------------------------------------------
1. Click the golden Genie Lamp in your menu bar at the top of your Mac screen.
2. You will see the prompt bar at the bottom: "Make a Wish..."
3. Type what you want to see, for example:
   - summon a monitor for cpu, gpu, and ram
   - grant a tracker for my weekly ai usage & quotas
   - manifest a gentle reminder to breathe, stretch & hydrate
   - grant a daily morning affirmation and mindful thought
4. Press Enter!
5. Watch your Genie build the widget in real time right in front of you.
6. When it finishes, you can click "Keep" to save it, or "Undo" to revert.


--------------------------------------------------------------------
5. TROUBLESHOOTING & COMMON QUESTIONS
--------------------------------------------------------------------

PROBLEM: The app says "Agent unavailable" when I make a wish.
FIX:
1. Baby Genie couldn't find an active AI tool in your Terminal.
2. Open Terminal and type "claude" or "codex" to make sure you are logged in.
3. In Baby Genie, click the Settings gear icon in the top-right header, 
   go to "Agents", and make sure Claude or Codex has a green status indicator.

PROBLEM: The lamp icon disappeared from my menu bar.
FIX:
If you have a MacBook with a screen notch or many menu bar icons, 
macOS might temporarily hide icons on the left.
1. Close a few unused background menu apps to free up space, or
2. Open Spotlight (Cmd + Space), type "Baby Genie", and press Enter to bring it forward.

PROBLEM: How do I quit or restart Baby Genie?
FIX:
Click the Genie lamp in the menu bar, then click the Power icon (⏻) 
in the top-right header to quit cleanly.
