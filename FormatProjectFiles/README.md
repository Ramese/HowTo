# .editorconfig

Place your .editorconfig file to every solution. Based on this file your solution will be formated. More information:  

[https://editorconfig.org/](https://editorconfig.org/)


## Used rules

  root = true

  [*]
  charset = utf-8
  indent_style = tab
  indent_size = 2
  tab_width = 2
  end_of_line = crlf
  insert_final_newline = true
  trim_trailing_whitespace = true
  
  [*.yml]
  indent_style = space
  indent_size = 2
  tab_width = 2
  end_of_line = crlf

## Use

### Visual Studio (.Net)

It finds the rules and applies them itself. There may be a problem with VS, but you can run it manually by using commnad:  

`dotnet format --verify-no-changes Solution.sln`


### Visual Studio Code

You can run manually using for example Angular CLI:  

`ng lint`

Doesn't work with .editconfig by default. It needs prettier plugin to be installed.
