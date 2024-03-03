<p align="center">
    <a href="https://doc.anytype.io">
        <img src=".gitbook/assets/anytype-logo-360px.png" alt="Docs-Logo" width="100px" height="100px">
    </a>
</p>


## Table of Contents

- [**Intro**](#Intro)
- [**Contribution process**](#contribution-process)
- [**File Structure**](#file-structure)
- [**Conventions**](#conventions)
  - [**Text Formats**](#text-formats)
  - [**Lists**](#lists)
  - [**Blocks**](#blocks)
  - [**Media**](#media)

## Intro

ℹ️ We ask that all users read our [Code of Conduct](https://github.com/anytypeio/community/blob/main/README.md#code-of-conduct) and [Gitbook Conventions](#conventions) before contributing to the documentation.
You are welcome to propose any changes in PR and participate in discussion in [Improvements for doc.anytype.io](https://community.anytype.io/t/improvements-for-doc-anytype-io/2862) topic. Please follow the steps below to contribute. If you're new to \_git\* and/or _GitHub_, we suggest you go through [the GitHub Guides](https://guides.github.com/introduction/flow/). 


## Contribution process

1. Fork this repository
2. (Optional) Clone the fork
   - Using SSH
     ```shell
     git clone --filter=tree:0 git@github.com:anytypeio/community.git
     ```
   - Using HTTPS
     ```shell
     git clone --filter=tree:0 https://github.com/anytypeio/community.git
     ```
   - Using GitHub CLI
     ```shell
     gh repo clone anytypeio/community -- --filter=tree:0
     ```
3. Create a new branch from the latest `main`
4. Make your changes on the new branch
5. Commit and push to the new branch
6. Make a pull request
7. Assign [Vladimir](https://github.com/d1eselboy), [Divyanshu](https://github.com/div3xi) or [Enda](https://github.com/endac) as the PR reviewer

## File Structure

* Any Page that has been added or removed from the documentation needs to be added to the **Table Of Contents** in the file [SUMMARY.md](https://github.com/anytypeio/docs/blob/main/SUMMARY.md)
  * Indentation is used to signify nesting of pages
  * Pages are linked using markdown URL's, e.g.:
    ```
    [Navigation](https://github.com/anytypeio/docs/blob/main/features/navigation.md)
    ```
* All files are saved as **Markdown .md**
* For nesting pages, they need to be placed in the category folder. If it does not exist, then you can create the folder
* To use images, they must all be placed inside the [.gitbook/assets](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) folder and then referenced from that folder
    > All media should be in light mode
## Conventions

> These are the rules that Gitbook follows while creating documentation from markdown. Please follow them while making any changes.

### Text Formats

- # Heading 1
  ```
  # Heading 1
  ```
  
- ## Heading 2
  ```
  ## Heading 2
  ```
  
- ### Heading 3
  ```
  ### Heading 3
  ```
  
- **Bold**
  ```
  **Bold Text**
  ```
  
- *Italics*
  ```
  _Italics Text_
  ```
  
- ~~Strikethrough~~
  ```
  ~Strikethrough Text~
  ```
  
- Horizontal Rule
  ```
  ---
  ```
  
- [URL](#)
  ```
  [URL Name](https://example.com)
  ```

- ![Image](#)
  ```
  ![Image](http://url/a.png)
  ```

- `Inline Code`
  ```
  `Inline Code`
  ```

### Lists

- **Un-Ordered List**
  ```
  * Item 1
  * Item 2
  * Item 3
      or
  - Item 1
  - Item 2
  - Item 3
  ```

- **Ordered List**
  ```
  1. Item 1
  2. Item 2
  3. Item 3
  ```

- **Task List**
  ```
  * [ ] Un-checked Task
  * [x] Checked Task
  ```
  
### Blocks

- **Code Blocks**
```
``` creates a new code block.
```py creates a new code block with Python syntax highlighting.
```

- **Quotes**
  ```
  Use > to start a quote block.
  ```

- **Information Hint Block**
  ```
  {% hint style="info" %} Information Hint Block {% endhint %}
  ```
  <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/info-hints-block.png" alt="info-hints">
    </a>
  </p>
  
- **Warning Hint Block**
  ```
  {% hint style="warning" %} Warning Hint Block {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/warning-hints-block.png" alt="warning-hints">
    </a>
  </p>
  
- **Success Hint Block**
  ```
  {% hint style="success" %} Success Hint Block {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/success-hints-block.png" alt="success-hints">
    </a>
  </p>
  
- **Danger Hint Block**
  ```
  {% hint style="danger" %} Success Hint Block {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/danger-hint-block.png" alt="danger-hints">
    </a>
  </p>

### Media

- **Block:** To create a Media Block, you need to use the below convention
  ```
  ![Media Caption](<.gitbook/assets/file-name>)
  
  E.g.:
  
  ![Home page](<.gitbook/assets/Screenshot 2021-11-05 at 18.45.31.png>)
  ```
  When adding a media block, if the page to which you are adding is nested, use `../` the appropriate number of times to make the embeds work.

- **File Storage :** Any media has to be uploaded to the [.gitbook/assets/](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) folder first. Only then it can be used inside the documentation. You may see GitBook embedding proprietary format `{% embed url=" in existing pages, you don't need to use that. 

- **File Formats:** These are the only file formats accepted for uploading media in the documentation.
    - **Videos:**
    
      > ✔️ Use only **MP4**
      > ❌ No **gifs** or other formats
      
    - **Images:**
      
      > ✔️ Use only **PNG** and **JPG** images
      > ❌ No other formats

- **Size Limits:**  There is a size limit of **5 MegaBytes** for each media file uploaded. 1000px wide images and videos can still be very legible, reducing 4k file size by probably 75%. 

- **Naming:** To reduce confusion, when uploading, please rename your files in a human-readable format
  ```
  <image-caption>-<page>.<file-format>
  
  E.g:
  ✔️ loadingscreen-intro.png
  ❌ Screenshot 2021-11-05 at 18.45.31.png
