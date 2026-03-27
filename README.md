# DearMarkdown
Markdown for Dear ImGui (md4c) 

## Use example

```cpp

#include "markdown.hpp"

void example() {
  std::string markdownText = R"(
#H1 Header : Text and Links
You can add [links like this one to enkisoftware](https://infinite.si/)
and lines will wrap well. You can also insert images ![image alt text](image
identifier e.g. filename) Horizontal rules:
***
___
*Emphasis* and **strong emphasis** change the appearance of the text.
## H2 Header: indented text.
  This text has an indent (two leading spaces).
    This one has two.
### H3 Header: Lists
  * Unordered lists
    * Lists can be indented with two extra spaces.
  * Lists can have [links like this one to Avoyd](https://www.avoyd.com/) and
*emphasized text*
)";

  ImGui::MarkdownView(markdownText);
}
```

## Credits


[Martin Mitáš](http://github.com/mity) : MD4C

[Dmitry Mekhontsev](https://github.com/mekhontsev) : md4c integration for Dear ImGui 

Original project for the Dear ImGui integration: imgui_md: Markdown for Dear ImGui using MD4C (https://github.com/mekhontsev/imgui_md)