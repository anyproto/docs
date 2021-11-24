 # Architecture and Fundamentals   
Are you now ready to move your entire workflow over to Anytype? Sounds great... but there are a few things that you&#39;ll need to understand first.   
   
Notion and Anytype operate based on two different architectures. This might sound scary, but once you grasp it, you&#39;ll be able to use Anytype like you use Notion right now in no time. Read on to find out more.   
   
 # The Page Canvas and Blocks   
If you&#39;ve used Notion and its Pages and Blocks, you&#39;ll have no difficulty in understanding Anytype&#39;s equivalent, which is its Object Canvas and Blocks.   
Each object has a canvas, and blocks can be placed within it.   
 ## Create a Block   
Notion&#39;s command pallete works almost exactly like Anytype&#39;s. Use the forward slash `/` to open the command pallete. Type to search, use the arrow keys to navigate up and down, or scroll through the list with your mouse. Press Enter, or click on the block type that you want, in order to create the desired block. By default, when you start typing on an Anytype object canvas, the block type will be plain text.   

![image.png](.gitbook/slashmenu.png)    

*To see a list of all available blocks, please refer to the Documentation page.*   
Want to create a block between, below, or even above another block? With Notion, you&#39;d have used the `+` button to only create a block below the current block.   
![image.png](.gitbook/notionblocks.png)    

Anytype&#39;s system is more flexible. Hover over the block dragger (shaped like a pill with three dots inside it), and a `+` button will pop out to your left.   
![image.png](.gitbook/anytypeblocks.png)    

Move your mouse over to the `+` button that just appeared, and you&#39;ll see a yellow line appear. This line indicates where your new block will be inserted. Click the `+`  button, and a new block will be created where the line is located.   
[Screen Recording 2021-11-14 at 10.20.41 AM.mov](.gitbook/anytypeaddingblocks.mp4)    
With this, you can create a block below or between preexisting blocks, but unli
ke Notion, you can also create a block above another block.   
To see options available for a block, such as deletion and duplication, click on the block dragger.   
![image.png](.gitbook/blockoptions.png)    
   
 ## Moving Blocks   
Blocks can be moved around freely around a Notion page. Similarly, blocks can also be moved freely around an Anytype page. They can go below, above, inside or even next to other blocks!    

To move blocks around an Anytype page, use the three-dotted dragger that appears once you hover over a block to click, then drag the block around a page - just like how&#39;d you use the dragger in Notion. You can also select or command-click to manipulate multiple objects at once!   
[Screen Recording 2021-11-14 at 10.28.13 AM.mov](.gitbook/movingblocks.mp4)    
There are some differences, however. You can also indent blocks within other blocks by directly dragging a block over another block in Anytype.   
   
 # Hierarchy, Page Linking, and Backlinks   
Notion&#39;s pages operate in a **hierarchical** manner, like your computer&#39;s file system. 

In your computer&#39;s file browser, folders **store** other folders and files. You can create shortcuts (or symbolic links) to refer to these files outside of the hierarchy. If you delete a folder, all the folders and files contained within it will be deleted, and shortcuts to those files will be broken.   
Similarly, in Notion, pages **store** other pages. You can also create backlinks to refer to pages outside of the hierarchy. Therefore, if you delete a page, all the pages contained within it will be deleted, along with backlinks referring to that page.   
   
[Screen Recording 2021-11-14 at 1.18.36 AM.mov](.gitbook/notionfs.mp4)    
Anytype operates in a fundamentally different manner. Rather than working like your computer&#39;s file system, it operates like the World Wide Web.   
Any website from the World Wide Web can **link** to another website. Every link is a shortcut, as links don&#39;t **store** other webpages; they just refer to them. If you delete a webpage or a link, the webpages that it linked to won&#39;t be affected or deleted. Other shortcuts will continue to work.   
Similarly, in Anytype, other objects (pages in Notion&#39;s lingo) can link to another object. This is how you organize other objects within your current object. If you delete links within an object or the object itself, the objects that it linked to won&#39;t be deleted, and other links to that object in other objects will continue to function.   
> To see which objects your current object links to, click on the Navigation button. Alternatively, click on the Graph button to see a full-featured graph showing all the links between your objects.   

That&#39;s also why backlinks in Notion are not a separate link type in Anytype - every link is a backlink.   
Relations also link objects together with another. You&#39;ll learn more about this in later sections.   
 ### **What does this mean for me?**   
Anytype&#39;s object linking architecture is more flexible than Notion&#39;s. You may be offput by the different architecture, but coming from a user who switched his entire workflow over from Notion to Anytype, you&#39;ll come to understand the benefits in no time.   
Having objects (or pages, if that&#39;s what you prefer) not be locked inside a hierarchical silo, but instead linked together in a knowledge graph brings numerous advantages. You no longer need to think about \*where\* an object belongs in your tree or where to place it, you simply link it. This allows for a much more natural flow of information compared to storing data inside a hierarchical note system.   
So, think of this scenario. You create an object, called &#34;Places I want to go to&#34;. You want to reference the &#34;Places I want to go to&#34; object in two other objects: Beautiful Scenery and     
   
If you want to read further about the advantages and disadvantages a non-hierarchical architecture brings to Anytype, I highly recommend reading this article: [https://www.nayuki.io/page/designing-better-file-organization-around-tags-not-hierarchies ](https://www.nayuki.io/page/designing-better-file-organization-around-tags-not-hierarchies)and https://www.nateliason.com/blog/roam   
 # Databases   
Notion&#39;s relational databases are an incredibly flexible tool to help you categorize, organize, and **store** database entries - each of which is a fully-functioning page. Anytype works differently, yet, you can achieve the same (and more) with Anytype&#39;s Sets, Types and Relations.   
 ## Sets and Relations   
![image.png](.gitbook/notiondb.png)    
*Here&#39;s a Notion database. Each database entry is a page, and has predefined **properties, such as Tags, URL, and Phone**.*   
   
Anytype&#39;s equivalent to Notion&#39;s databases are Sets. Unlike Notion databases, Sets do not **store** objects. Instead, they **show**, not store, all objects which meet a specific criteria, kind of how search works. Currently, sets can only show objects with one specific Type relation. Don&#39;t know what a Relation is? We&#39;ll cover it shortly.   
This makes Anytype much more flexible than Notion. With Notion, if you wanted to create a database, you are stuck with it. You cannot move pages outside of the database, nor can you bring pages inside of a database once they have already been created (without annoying workarounds and time-wasting steps.) Instead, with Anytype, you can bring **any** existing object in view with a Set.   
Learn more about Types and Sets here-&gt;   
   
*Here&#39;s an Anytype set. Right now, it&#39;s configured to show all Objects with the relation `To-Do.`*   
![Demo of sets](.gitbook/setdemo.png)
<details> Having trouble understanding Anytype's databases? Click here to see a simplified explanation.   

- Think of an individual Notion database within Anytype as a Type.    
-    
- To create a &#34;database&#34; in Anytype, first, create a Type, then create a new Set to show all objects of that Type.  
  
</details>
   
 ## Relations   
In Notion&#39;s databases, you may be familliar with properties, which are attributes connected to each database entry to describe it. In Anytype, relations (Anytype&#39;s equivalent of properties) are not only applied to individual database entries, but applied to **every single object**. Relations describe each Object. Many Notion properties are also applicable to Anytype&#39;s relations, such as tags, URL, phone number, last modified by, descriptions, checkboxes, and much more. Find out more about Relations in the documentation page.   
Relations can be defined for a Type. This is the equivalent as using the `+` button in a Notion database to create a new property.   
![image.png](.gitbook/anytyperelations.png)    
   
   
![image.png](.gitbook/notionrelations.png)    
You can configure a Set to show relations (properties in Notion&#39;s lingo). Furthermore, you can create different Views (like Notion) that have different filtering and sorting settings, based on the Relations of the object.    
Filtering, sorting and creating views in a Set work in a very similar manner to Notion, so you shouldn&#39;t have much trouble getting things sorted out. Check out the documentation on Sets for more information.   
<details> Having trouble understanding Relations in contrast to Notion's Databases? Click here for a simplified explanation. 

- Consider Anytype&#39;s Relations to be Attributes within a Notion database.   
- When you add an attribute to a Notion database, you use the `+` button to the right of the column header.   
![image.png](.gitbook/basicstep1.png)    
- Instead, in Anytype, to add an attribute to a database, open the Library (square menu on the home screen) and click on the &#34;Types&#34; tab. Open the desired Type and add attributes - known as relations in Anytype&#39;s lingo.   
![image.png](.gitbook/basicstep2.png)    
- Click &#34;Create&#34;, then select Set of object to create a database view.   
- Click the Options button to add the Relations (Attributes) to the database view.   
![image.png](.gitbook/basicstep3.png)    
  
  </details>
   
 ### What does this mean for me?   
Anytype&#39;s equivalent of Notion&#39;s databases may not seem quite as straightforward, but, once you understand exactly how they work, they may end up being a more powerful and flexible tool than Notion&#39;s databases.   
   
 # Templates   
 In progress...
