---
hide:
  - tags
  - footer
tags:
  - Scripting
  - Script
---

# **Scripting**


{==

## **Installing a Script**

==}


---


{==

## **Sample Scripts**

==}

**Paragraph Styles**

```jsx
//First, check to see if the paragraph style already exists.
var myParagraphStyle = myDocument.paragraphStyles.item("2021");
try {
    var myName = myParagraphStyle.name;
}
catch (myError){
    //The paragraph style did not exist, so create it.
    myParagraphStyle = myDocument.paragraphStyles.add({name:"Heading 1"});
}
```

---

**Delete EVERYTHING from the pasteboard**

```jsx
var pasteboardItems = [];
var spreadRef = app.activeWindow.activeSpread;
var itemList =  spreadRef.pageItems.everyItem().getElements();
var thisItem, myParent;
for (var i = 0; i < itemList.length; i++) {
    thisItem = itemList[i];
    myParent = thisItem.parentPage;
    if (myParent == null) {
        // Add object to list named "pasteboardItems"
        // pasteboardItems.push(thisItem);
        thisItem.remove();
    }
}
pasteboardItems;
```

---

**Delete ALL unused swatches**

```jsx
function deleteAllUnusedSwatches(){
	while (myDocument.unusedSwatches[0].name != "") {
	    id = myDocument.unusedSwatches[0].id;
	    sw = myDocument.swatches.itemByID(id);
	    sw.remove();
	}
}
deleteAllUnusedSwatches()
```

**OR**

```jsx
var myUnusedSwatches = myDocument.unusedSwatches;
for (var s = myUnusedSwatches.length-1; s >= 0; s--) {
    var mySwatch = myDocument.unusedSwatches;
    var mySwatchName = mySwatch.name;
    // alert (mySwatchName);
    if (mySwatchName != ""){ mySwatch.remove(); }}
```


---
