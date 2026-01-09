# CLAUDE.md - Alba Parent Portal

## Purpose
Read-only parent portal to view Alba's learning progress. Pulls data from the same Gist as AEA-V2.

---

## 🚨 CRITICAL RULES

### 1. READ-ONLY
This portal only READS from Gist. It NEVER writes. Any write functionality must go in AEA-V2, not here.

### 2. SEPARATE ENVIRONMENTS
| Environment | URL | Gist ID |
|-------------|-----|---------|
| **Production** | https://spike1990ai.github.io/alba-parent-portal/ | `3cdae715fe2eb3b76b17fa98212fec3e` |
| **Staging** | https://spike1990ai.github.io/alba-parent-portal-staging/ | `c7d833305a1f527c65da66978ed82a06` |

### 3. NO BUILD STEP
This is static HTML + Tailwind CDN. No npm, no React, no build process.

---

## Deploy

```bash
# Production
cd /path/to/alba-parent-portal
git add . && git commit -m "Update" && git push

# Staging
cd /path/to/alba-parent-portal/staging
git add . && git commit -m "Update" && git push
```

GitHub Pages deploys automatically on push to main.

---

## Files

```
alba-parent-portal/
├── index.html      # Production portal
├── CLAUDE.md       # This file
└── staging/
    └── index.html  # Staging portal (separate git repo)
```

---

## PIN
Parent PIN: `3521` (same as AEA-V2)

---

## Related Projects
- **AEA-V2** - Main learning app (Alba's phone)
- **AEA-V2-staging** - Staging version of learning app
