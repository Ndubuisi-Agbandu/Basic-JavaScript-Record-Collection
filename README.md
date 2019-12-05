# Basic-JavaScript-Record-Collection
This is the record collection task i did in freecodecamp during my hundred days of code.

### The Challenge
You are given a JSON object representing a part of your musical album collection. Each album has several properties and a unique id number as its key. Not all albums have complete information.

Write a function which takes an album's **id** (like **2548**), a property **prop** (like **"artist"** or **"tracks"**), and a **value** (like **"Addicted to Love"**) to modify the data in this collection.

If **prop** isn't **"tracks"** and **value** isn't empty (**""**), update or set the **value** for that record album's property.

Your function must always return the entire collection object.

#### There are several rules for handling incomplete data:

If **prop** is **"tracks"** but the album doesn't have a **"tracks"** property, create an empty array before adding the new **value** to the album's corresponding property.

If **prop** is **"tracks"** and **value** isn't empty (**""**), push the **value** onto the end of the album's existing **tracks** array.

If **value** is empty (**""**), delete the given **prop** property from the album.

#### Note:

1. You should not change the **collection** object's initialization
1. After **updateRecords(5439, "artist", "ABBA"), artist** should be **"ABBA"**
1. After **updateRecords(5439, "tracks", "Take a Chance on Me"), tracks** should have **"Take a Chance on Me"** as the last element.
1. After **updateRecords(2548, "artist", ""), artist** should not be set
1. After **updateRecords(1245, "tracks", "Addicted to Love"), tracks** should have **"Addicted to Love"** as the last element.
1. After **updateRecords(2468, "tracks", "Free"), tracks** should have **"1999"** as the first element.
1. After **updateRecords(2548, "tracks", ""), tracks** should not be set
1. After **updateRecords(1245, "album", "Riptide"), album** should be **"Riptide"**
