---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
---


<script src="https://cdnjs.cloudflare.com/ajax/libs/marked/4.3.0/marked.min.js"></script>
<div id="content">Loading...</div>
<script>
    async function loadMarkdown() {
        const url = "https://raw.githubusercontent.com/UntitledOutput/UntitledOutput/refs/heads/main/README.md";
        const response = await fetch(url);
        const text = await response.text();
        document.getElementById("content").innerHTML = marked.parse(text);
    }
    loadMarkdown();
</script>

