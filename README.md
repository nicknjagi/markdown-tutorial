# Summary of Markdown Syntax

- [Summary of Markdown Syntax](#summary-of-markdown-syntax)
  - [Headings](#headings)
  - [Paragraphs](#paragraphs)
    - [Line breaks](#line-breaks)
  - [Emphasis](#emphasis)
    - [Bold](#bold)
    - [*Italic*](#italic)
    - [Bold and *Italic*](#bold-and-italic)
  - [Blockquotes](#blockquotes)
    - [Blockquotes with multiple paragraphs](#blockquotes-with-multiple-paragraphs)
    - [Nested blockquotes](#nested-blockquotes)
    - [Blockquotes with Other Elements](#blockquotes-with-other-elements)
  - [Lists](#lists)
    - [Ordered lists](#ordered-lists)
    - [Unordered lists](#unordered-lists)
    - [Starting Unordered List Items With Numbers](#starting-unordered-list-items-with-numbers)
  - [Adding elements in lists](#adding-elements-in-lists)
    - [Nesting Lists](#nesting-lists)
  - [Code Blocks](#code-blocks)
  - [Fenced Code Blocks](#fenced-code-blocks)
  - [Syntax Highlighting](#syntax-highlighting)
  - [Images](#images)
  - [Code](#code)
  - [Horizontal Rules](#horizontal-rules)
  - [Links](#links)
  - [Linking Images](#linking-images)
  - [Adding Titles](#adding-titles)
  - [URLs and Email Addresses](#urls-and-email-addresses)
  - [Formatting Links](#formatting-links)
  - [Escaping Characters](#escaping-characters)
  - [Tables](#tables)
    - [Alignment](#alignment)
  - [Task List](#task-list)
  - [Useful resources](#useful-resources)
____

## Headings

To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three `<h3>`, use three number signs (e.g., ### My Header)

    # Heading level 1 // --> <h1></h1>
    # Heading level 2 // --> <h2></h2>
    # Heading level 3 // --> <h3></h3>
    # Heading level 4 // --> <h4></h4>
    # Heading level 5 // --> <h5></h5>
    # Heading level 6 // --> <h6></h6>

>**Best practice**
> Try to put a blank line before and after a header.

## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

*Don't put tabs or spaces in front of your paragraphs.*

*Keep lines left-aligned like this.*

### Line breaks

First line with two spaces after.  
And the next line.

First line with the HTML tag `<br>`after.<br>
And the next line.

## Emphasis

### Bold

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

    I just love **bold text**
or

    I just love __bold text__.

**Rendered Output**

I just love **bold text**

    love**is**bold

**Result** > Love**is**bold

### *Italic*

    Italicized text is the *cat's meow*.

**Result**

Italicized text is the *cat's meow*.

### Bold and *Italic*

**Markdown**

    This text is ***really important***.
    This text is ___really important___.
    This text is __*really important*__.
    This text is **_really important_**.

**Result**

This text is ***really important***.

## Blockquotes

To create a blockquote, add a `>` in front of a paragraph.

    > Dorothy followed her through many of the beautiful rooms in her castle.

**Result**

> Dorothy followed her through many of the beautiful rooms in her castle.

### Blockquotes with multiple paragraphs

Add a `>` on the blank lines between the paragraphs.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

**Result**

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### Nested blockquotes

Add a `>>` in front of the paragraph you want to nest.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

**Result**

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.


### Blockquotes with Other Elements

    > #### The quarterly results look great!
    >
    > - Revenue was off the chart.
    > - Profits were higher than ever.
    >
    >  *Everything* is going according to **plan**.

**Result**

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going according to **plan**.

> **Best practice**
> Try to put a blank line before and after a blockquote.

## Lists

### Ordered lists

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one

`1. First item`
`2. Second item`
`3. Third item`
`4. Fourth item`

### Unordered lists

To create an unordered list, add dashes `-`, asterisks `*`, or plus signs `+` in front of line items. Indent one or more items to create a nested list.

    - First item
    - Second item
    - Third item
    - Fourth item

**Result**

- First item
- Second item
- Third item
- Fourth item
  
### Starting Unordered List Items With Numbers

If you need to start an unordered list item with a number followed by a period, you can use a backslash `\` to escape the period.

    - 1968\. A great year!

**Result**

- 1968\. A great year!

## Adding elements in lists

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples

**Paragraphs**

    * This is the first list item.
    * Here's the second list item.

        I need to add another paragraph below the second list item.

    * And here's the third list item.
  
**Result**

* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.

**Blockquote**

    * This is the first list item.
    * Here's the second list item.

        > A blockquote would look great below the second list item.

    * And here's the third list item.

**Result**

* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list item.

* And here's the third list item.
 
### Nesting Lists

    1. First item
    2. Second item
    3. Third item
        - Indented item
        - Indented item
    4. Fourth item

**Result**

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

## Code Blocks

Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

    1. Open the file.
    2. Find the following code block on line 21:

            <html>
              <head>
                <title>Test</title>
              </head>

    3. Update the title to match the name of your website.

**Result**

1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

## Fenced Code Blocks

The basic Markdown syntax allows you to create code blocks by indenting lines by four spaces or one tab. If you find that inconvenient, try using fenced code blocks. Depending on your Markdown processor or editor, you’ll use three backticks (```) or three tildes (~~~) on the lines before and after the code block. The best part? You don’t have to indent any lines!

    ```
    {
    "firstName": "John",
    "lastName": "Smith",
    "age": 25
    }
    ```

**result**

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## Syntax Highlighting

To add syntax highlighting, specify a language next to the backticks before the fenced code block.

    ```json
    {
    "firstName": "John",
    "lastName": "Smith",
    "age": 25
    }
    ```

**Result**

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## Images

To add an image, add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses. You can optionally add a title in quotation marks after the path or URL.

      1. Open the file containing the Linux mascot.
      2. Marvel at its beauty.

          ![Tux, the Linux mascot](/assets/images/tux.png)

      3. Close the file.
       
**Result**

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/tux.avif)

3. Close the file.


## Code

To denote a word or phrase as code, enclose it in backticks (`)

    At the command prompt, type `nano`.

**Result**

At the command prompt, type `nano`.

## Horizontal Rules

---

To create a horizontal rule, use three or more asterisks `***`, dashes `---`, or underscores `___` on a line by themselves.

## Links

To create a link, enclose the link text in brackets (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., (https://duckduckgo.com)).


    My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

**Result**

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

## Linking Images

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

    [![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

## Adding Titles

You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in quotation marks after the URL.

    My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").

**Result**

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").


## URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

    <https://www.markdownguide.org>
    <fake@example.com>

**Result**

<https://www.markdownguide.org>
<fake@example.com>

## Formatting Links

To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

    I love supporting the **[EFF](https://eff.org)**.
    This is the *[Markdown Guide](https://www.markdownguide.org)*.
    See the section on [`code`](#code).

**The Result**

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash `\` in front of the character.

## Tables

To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate each column. For compatibility, you should also add a pipe on either end of the row.

    | Syntax      | Description |
    | ----------- | ----------- |
    | Header      | Title       |
    | Paragraph   | Text        |

**Output**

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

### Alignment

You can align text in the columns to the left, right, or center by adding a colon (:) to the left, right, or on both side of the hyphens within the header row.

    | Syntax      | Description | Test Text     |
    | :---        |    :----:   |          ---: |
    | Header      | Title       | Here's this   |
    | Paragraph   | Text        | And more      |

**Output**

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

## Task List
 In Markdown applications that support task lists, checkboxes will be displayed next to the content. To create a task list, add dashes (-) and brackets with a space ([ ]) in front of task list items. To select a checkbox, add an x in between the brackets ([x]).

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

**Output**

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media.


## Useful resources

Visit [markdownguide.org](https://www.markdownguide.org/) for more information.


