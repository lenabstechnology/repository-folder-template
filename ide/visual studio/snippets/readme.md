# Visual Studio Code Snippets

Code snippets are small blocks of reusable code that you can add to a code file by using the right-click context menu command or a combination of hotkeys. Microsoft official documentation [here](https://learn.microsoft.com/en-us/visualstudio/ide/code-snippets?view=vs-2022)

## Create a code snippet

1. Start Visual Studio. Then, in the **Get started** section of the Start window, select **Continue without code**.
2. From the menu bar, select **File > New > File** (or, enter the keyboard shortcut **Ctrl+N**) to open the **New File** dialog. Then, select **XML File**.
3. Add the template code shown in the [Snippet template](#snippet-template) section below.
4. In the code, fill in the title of the snippet in the **Title** element. Use the title **My Snippet**.
5. Fill in the language of the snippet in the **Language** attribute of the **Code** element. For C#, use **CSharp**, for Visual Basic, use **VB**, and for C++, use **CPP**.
6. Add the snippet code in the **CDATA** section inside the **Code** element.
7. Save the snippet as **MySnippet.snippet** (you can save it anywhere).


## Snippet Template

The following XML is the basic snippet template.

```xml
<?xml version="1.0" encoding="utf-8"?>
<CodeSnippets xmlns="http://schemas.microsoft.com/VisualStudio/2005/CodeSnippet">
    <CodeSnippet Format="1.0.0">
        <Header>
            <Title></Title>
        </Header>
        <Snippet>
            <Code Language="">
                <![CDATA[]]>
            </Code>
        </Snippet>
    </CodeSnippet>
</CodeSnippets>
```

## Import a code snippet

1. You can import a snippet to your Visual Studio installation by using the **Code Snippets Manager**. Open it by selecting **Tools > Code Snippets Manager**.

2. Select the **Import** button.

3. Go to the location where you saved the code snippet in the previous procedure, select it, and select **Open**.

4. The **Import Code Snippet** dialog opens, asking you to choose where to add the snippet from the choices in the right pane. One of the choices should be **My Code Snippets**. Select it, select **Finish**, and then select **OK**.

5. The snippet is copied to one of the following locations, depending on the code language and the version of Visual Studio that you're using:

    * *%USERPROFILE%\Documents\Visual Studio %VERSION%\Code Snippets\Visual C#\My Code Snippets*
    * *%USERPROFILE%\Documents\Visual Studio %VERSION%\Code Snippets\Visual Basic\My Code Snippets*

    > Note that, you should replace **"*%USERPROFILE%*"** and **"*%VERSION%*"** values in path with yours.
    > eg. *JEPOZDEMIR\Documents\Visual Studio 2022\Templates\ItemTemplates*


## Test your snippet

* Test your snippet by opening a C# or Visual Basic project. With a code file open in the editor, choose **Snippets > Insert Snippet** from the right-click menu, then **My Code Snippets**. You should see a snippet named **My Snippet**. Double-click it.

* The snippet code is inserted in the code file.

