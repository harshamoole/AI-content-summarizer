# 🧠 AI Content Summarizer Plugin for WordPress

A simple WordPress plugin that uses OpenAI's GPT-3.5 to automatically summarize blog posts inside the WordPress editor.

---

## ✨ Features

- Adds a "Summarize with AI" button to the post editor
- Sends content to OpenAI and adds the summary to the excerpt
- Uses `fetch()` + AJAX for live summaries
- Lightweight and easy to modify

---

## 🔧 How It Works

1. Write a post in the WordPress block editor.
2. Click the "✨ Summarize with AI" button near the post title.
3. The plugin calls the OpenAI API and inserts the summary as the post excerpt.

---

## 🚀 Installation

1. Clone/download the repo into `wp-content/plugins/ai-content-summarizer/`
2. (Optional) Run `npm install` if you plan to extend or compile scripts
3. Activate the plugin from WordPress Admin → Plugins

---

## 🔐 Configuration

Replace this line in `ai-content-summarizer.php`:

```php
$api_key = getenv('OPENAI_API_KEY');
