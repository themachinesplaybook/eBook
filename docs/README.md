# The Machine's Playbook - Website

This is the GitHub Pages website for "The Machine's Playbook" with enhanced chat UI styling for Dave & Eve conversations.

## 🚧 Status: In Development

**What Works:**
- ✅ Landing page (index.html)
- ✅ Chapter navigation
- ✅ CSS styling with chat UI components
- ✅ All 12 chapters converted to HTML
- ✅ Mobile-responsive layout

**In Progress:**
- ⚠️ Conversation parser needs refinement to properly detect and wrap Dave/Eve dialogues in chat bubbles
- ⚠️ Currently conversations render as plain text, not styled chat UI

## 📂 Structure

```
docs/
├── index.html              # Landing page
├── css/
│   └── style.css          # All styling including chat UI
├── chapters/              # All 12 chapters as HTML
│   ├── 00-introduction.html
│   ├── 01-the-first-spin.html
│   └── ... (12 total)
└── README.md
```

## 🎨 Chat UI Design

The CSS includes beautiful chat bubble styling:
- Dave's messages: Right-aligned, blue bubbles
- Eve's messages: Left-aligned, grey bubbles with green name
- Familiar messaging app interface

**Once conversation parser is fixed, conversations will look like ChatGPT/iMessage**

## 🔧 Build Process

Build website from markdown sources:
```bash
python3 build_website.py
```

This converts markdown chapters in `outputs/clean/final/` to HTML in `docs/chapters/`

## 🌐 GitHub Pages

**Note:** GitHub Pages requires a PUBLIC repository on free tier.

This repo is currently PRIVATE, so Pages won't be accessible yet.

**To enable:**
1. Make repository public (when ready to launch)
2. Go to Settings → Pages
3. Source: Deploy from branch
4. Branch: master, Folder: /docs
5. Save

**URL will be:** `https://xeeva.github.io/The-Machines-Playbook/`

## 🔄 Next Steps

1. Refine conversation parser to properly wrap `**Dave:**` and `**Eve:**` exchanges
2. Test chat UI rendering
3. Add en-AU spelling pass
4. Final review before making repo public
5. Enable GitHub Pages

## 📝 License

Same as main repository: CC BY-NC-SA 4.0
