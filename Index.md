# 🧭 Obsidian Vault Index

Welcome! Use this dynamic index to explore your vault. All content is grouped by category and auto-updated using Dataview.

```dataview
TABLE GIT_USERNAME, GIT_TOKEN
WHERE file.name = "credentials"
```
---

## 🔧 01_Reference – Tools & Cheat Sheets

```dataviewjs
const pages = dv.pages('"MyVault/01_Reference"')
	.groupBy(p => {
	    const folder = p.file.folder;
	    return folder === "MyVault/01_Reference/" ? "" 
	    : folder.replace("MyVault/01_Reference/", "");
	});

for (let group of pages) {
    dv.header(3, group.key);
    dv.list(group.rows.map(p => p.file.link));
}
```

---

## 🧠 02_Promts – Prompt Templates

```dataviewjs
const pages = dv.pages('"MyVault/02_Promts"')
	.groupBy(p => {
	    const folder = p.file.folder;
	    return folder === "MyVault/02_Promts" ? "" 
	    : folder.replace("MyVault/02_Promts/", "");
	});

for (let group of pages) {
    dv.header(3, group.key);
    dv.list(group.rows.map(p => p.file.link));
}
```

---

## 🚧 03_Projects – Work in Progress

```dataviewjs
const pages = dv.pages('"MyVault/03_Projects"')
	.groupBy(p => {
	    const folder = p.file.folder;
	    return folder === "MyVault/03_Projects" ? "" 
	    : folder.replace("MyVault/03_Projects/", "");
	});

for (let group of pages) {
    dv.header(3, group.key);
    dv.list(group.rows.map(p => p.file.link));
}
```

---

## 📜 04_Workflows – Step-by-Step Guides

```dataviewjs
const pages = dv.pages('"MyVault/04_Workflows"')
	.groupBy(p => {
	    const folder = p.file.folder;
	    return folder === "MyVault/04_Workflows" ? "" 
	    : folder.replace("MyVault/04_Workflow/", "");
	});

for (let group of pages) {
    dv.header(3, group.key);
    dv.list(group.rows.map(p => p.file.link));
}
```

---

