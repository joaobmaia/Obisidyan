---
id: <% tp.date.now("YYYYMMDDHHmmss") %>
criado: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
atualizado: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
tipo: <%*
    var folder = tp.file.folder(true);
    if (folder.includes("Bibliográfica")) {
        tR += "bibliográfica";
    } else if (folder.includes("Permanente")) {
        tR += "permanente";
    } else if (folder.includes("Índice")) {
        tR += "índice";
    } else {
        tR += "nota";
    }
%>
assunto: 
tags: 
estado: #rascunho
---

<%*
    var title = tp.file.title;
    var folderForTitle = tp.file.folder(true);
    
    if (folderForTitle.includes("Bibliográfica")) {
        title = "📚 " + title;
    } else if (folderForTitle.includes("Permanente")) {
        title = "💎 " + title;
    } else if (folderForTitle.includes("Índice")) {
        title = "🗂️ " + title;
    }
    tR += "# " + title;
%>