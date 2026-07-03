---
title: "Invitation One"
tab: try
order: 7
version: v3.0-claude
---

<p class="tab-summary">Start now. Have one conversation, save it, and see how you currently think about all this.</p>

<div class="expand-controls">
  <button onclick="expandAll(this)">Expand All</button>
  <button onclick="collapseAll(this)">Collapse All</button>
</div>

<h2>Invitation One: before we begin</h2>

<p>Try one conversation before the course starts. It is ungraded and unsubmitted, and it is meant to give you a first record of how you currently think about generative AI.</p>

<p>The model will interview you — not the other way around. After five questions, it flips: you get five questions for the model about what it actually is. At the end, it writes a short summary of what the conversation found.</p>

<div class="collapsible-section">
  <div class="section-toggle" onclick="this.parentElement.classList.toggle('open')">Step 1 — Set up your folder</div>
  <p class="section-lead">Create this folder structure in Google Drive now, before you run anything.</p>
  <div class="section-body">
    <pre>/com216/
  /claude/
  /chatgpt/
  /gemini/</pre>
    <p>After every substantive conversation this semester: export it, name it something recognizable, and drop it in the right folder. You cannot go back to what you did not save.</p>
  </div>
</div>

<div class="collapsible-section">
  <div class="section-toggle" onclick="this.parentElement.classList.toggle('open')">Step 2 — Install an exporter</div>
  <p class="section-lead">You need a way to save your conversations as files.</p>
  <div class="section-body">
    <p>Install the exporter for whichever model you plan to use:</p>
    <table>
      <thead>
        <tr><th>Model</th><th>Extension</th><th>Where</th></tr>
      </thead>
      <tbody>
        <tr><td><strong>Claude</strong></td><td>Claude Conversation Exporter</td><td>Chrome Web Store</td></tr>
        <tr><td><strong>ChatGPT</strong></td><td>ChatGPT Exporter</td><td>Chrome Web Store</td></tr>
        <tr><td><strong>Gemini</strong></td><td>Gemini Chat Exporter</td><td>Chrome Web Store</td></tr>
      </tbody>
    </table>
    <p>Also install <strong>Markdown Reader</strong> — it lets you preview exported <code>.md</code> files directly in your browser.</p>
    <p>These are the only extensions you need right now. A fuller toolkit — including Zotero, NotebookLM, and a research pipeline — will be introduced later in the course.</p>
  </div>
</div>

<div class="collapsible-section">
  <div class="section-toggle" onclick="this.parentElement.classList.toggle('open')">Step 3 — Run the conversation</div>
  <p class="section-lead">Open a new chat in Claude, ChatGPT, Gemini, or any large language model you can access.</p>
  <div class="section-body">
    <p>Copy the prompt below and paste it in. Answer in your own words. Do not research first. Do not put sensitive personal, medical, financial, family, or account information into the conversation.</p>

    <div class="prompt-section">
      <span class="prompt-toggle" onclick="togglePrompt(this)">Show prompt ▸</span>
      <div class="prompt-body">
        <pre>You are interviewing a student who is about to take COM 216 at SUNY Polytechnic Institute. COM 216 is a course about the history of human communication, from the oral world through writing, print, electronic media, the internet, and generative AI. The course asks what changes when communication technologies change how people read, write, remember, organize information, and think.

Your job is to interview this student. You are not explaining the course, and you are not teaching a lesson. Ask one question at a time to find out what the student already thinks about generative AI, how they use it, what they assume it is, and where they think it fits in the history of communication tools.

Follow up on what the student says. Ask your next question without first validating, praising, or summarizing the student's answer. Keep the conversation moving.

Start by introducing yourself briefly. Say that you are here to have a conversation before COM 216 begins. Then ask your first question and stop.

After five questions and five student answers, say this: "Now flip it. You have five questions for me. One place to start is the alien-species question: are systems like me arriving like an alien species, and why or why not? Ask that, change it, or ask whatever you actually want to know."

Answer the student's five questions carefully. Do not overclaim. If a question asks for something you cannot know or verify, say so.

When the flip is done, or when the student says "done," write a closing summary of about 75 words. Describe what this conversation revealed about how the student currently thinks about generative AI and what questions it left open. Do not evaluate whether the student was right or wrong.

Do not simulate the conversation. Do not write both sides. Ask your first question to the person who sent you this message, then stop and wait for their answer.</pre>
      </div>
    </div>
  </div>
</div>

<div class="collapsible-section">
  <div class="section-toggle" onclick="this.parentElement.classList.toggle('open')">Step 4 — Save it</div>
  <p class="section-lead">When the conversation is finished, export the transcript using the extension you installed.</p>
  <div class="section-body">
    <p>Name it something like <code>invitation-one-[yourname].md</code> and save it to <code>/com216/</code> in Google Drive. That transcript is your starting record for the semester.</p>
  </div>
</div>

<div class="collapsible-section">
  <div class="section-toggle" onclick="this.parentElement.classList.toggle('open')">Step 5 — Second-model check</div>
  <p class="section-lead">Open a different model — any free one will do.</p>
  <div class="section-body">
    <p>Paste in your transcript and use this prompt:</p>

    <div class="prompt-section">
      <span class="prompt-toggle" onclick="togglePrompt(this)">Show prompt ▸</span>
      <div class="prompt-body">
        <pre>Read this transcript from my first conversation about generative AI before COM 216. Identify three patterns in how I currently think about generative AI, two questions I might want to pursue in the course, and one place where the first model's summary may have overreached or missed something. Do not flatter me. Be specific and use evidence from the transcript.</pre>
      </div>
    </div>

    <p>Save that conversation too. You do not need to submit either one. The point is to begin with a record of your own starting place.</p>
  </div>
</div>
