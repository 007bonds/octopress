---
layout: page
title: "Github Style Codeblock"
date: 2011-07-26 23:42
sidebar: false
footer: false
---

With the `backtick_codeblock` filter you can use Github's lovely back tick syntax highlighting blocks.
Simply start a line with three back ticks followed by a space and the language you're using. Tab in four spaces
for your code snippets, and then finish your code block with three more back ticks.

#### Syntax

    ``` language
        code snippet
    ```

### Example

    ``` ruby
        class Fixnum
          def prime?
            ('1' * self) !~ /^1?$|^(11+?)\1+$/
          end
        end
    ```

``` ruby
    class Fixnum
      def prime?
        ('1' * self) !~ /^1?$|^(11+?)\1+$/
      end
    end
```

This is a nice, lightweight way to add a highlighted code snippet. For features like titles and links you'll want to look
at the `codeblock` or `include_code` liquid tags.
