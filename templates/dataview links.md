> [!info]+ Links
> ```dataview 
> TABLE without id
> map(file.outlinks, (link) => "[[" + meta(link).path + "]]") AS "Исходящие",
> map(file.inlinks, (link) => "[[" + meta(link).path + "]]") AS "Входящие"
> WHERE file.name = this.file.name
> ```