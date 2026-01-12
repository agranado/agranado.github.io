# Personal Website - Alejandro Granados

Modern Hugo-based personal website with PaperMod theme.

## Setup

### 1. Install Hugo

```bash
# macOS
brew install hugo

# Linux (Debian/Ubuntu)
sudo apt install hugo

# Or download from https://gohugo.io/installation/
```

### 2. Install PaperMod Theme

```bash
cd website-new
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

### 3. Add Your Images

Place screenshots in the appropriate folders:

```
static/images/
├── lloom/
│   └── header.png          # LLOOM architecture diagram
├── aria/
│   ├── header.png          # ARIA overview
│   ├── langgraph_loop.png  # State machine diagram
│   └── nmi_heatmap.png     # Agent vs human comparison
└── indica/
    ├── header.png          # Disease screening overview
    ├── fibroblast_atlas.png # Atlas UMAP
    └── forest_plot.png     # Disease enrichment results
```

### 4. Local Development

```bash
hugo server -D
# Open http://localhost:1313
```

### 5. Build for Production

```bash
hugo --minify
# Output in /public directory
```

### 6. Deploy to GitHub Pages

```bash
# Copy contents of /public to agranado.github.io repository
cp -r public/* ../agranado.github.io/
cd ../agranado.github.io
git add .
git commit -m "Update website"
git push
```

## Content Structure

```
content/
├── about.md              # About page
├── papers.md             # Publications
└── posts/
    ├── lloom-multi-agent-gsea.md
    ├── aria-single-cell-agent.md
    └── indica-disease-screening.md
```

## Images Needed

### LLOOM Article
- Architecture diagram showing 4 sub-agents
- Sample output (redacted if needed)

### ARIA Article
- LangGraph state machine diagram (Planner→Analyst→Executor→Reviewer loop)
- NMI heatmap comparing agent vs human annotations
- Sample HTML report screenshot (redacted)

### Indica Article
- Fibroblast atlas UMAP (can use public CZI data)
- Forest plot of disease enrichments
- Pipeline overview diagram

## Customization

Edit `config.toml` to change:
- Site title and description
- Social links
- Menu items
- Theme settings
