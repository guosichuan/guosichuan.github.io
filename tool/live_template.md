---
title: "IntelliJ Idea Live Template"
date: 2016-06-27 23:04
collection: "IDE"
---

#IntelliJ Idea Live Template
@(IntellJ IDEA)[idea, live template, simiki]


[TOC]


##预定义变量

| 变量名      |     功能 |  
| :--------: | :--------:|
|$END$|最后鼠标位置|
|$SELECTION$|在 surround templates 中代表选中的代码块|


##预定义函数


| 函数名      |     功能 |  
| :--------: | :--------|
| annotated("annotation qname")    |  Creates a symbol of type with an annotation that resides at the   pecified location. For an example, see Live Templates in the iterations group. |
| <font color=red>arrayVariable()</font>    | 返回当前范围内推荐的可用数组变量  |
| anonymousSuper()   | Suggests a supertype for a Kotlin object expression.  |
| camelCase(String)    | 转换成驼峰式  my-text-file/my text file/my_text_file => myTextFile.|
| capitalize(String)    |  首字母大写 |
| capitalizeAndUnderscore(sCamelCaseName)    |驼峰样式转换成大写并用下划线分割FooBar => FOO_BAR|
| castToLeftSideType()    |  返回等号左边定义的类型 |
| className(sClassName)    |   类名|
| classNameComplete()    |   This expression substitutes for the class name completion at the variable position.|
| clipboard()    |   粘贴剪切板|
| complete()    |   补全|
| completeSmart()    |   智能补全|
| <font color=red>componentTypeOf (<array variable or array type>)</fond>    |返回**数组**的成员类型   |
| currentPackage()    |   包名|
| date(sFormat)    | 当前系统时间|
|decapitalize(sName)|取消首字母大写|
|descendantClassEnum(<String>)|Shows the children of the class entered as a string parameter.|
|enum(sCompletionString1,sCompletionString2,...)|List of comma-delimited strings suggested for completion at the template invocation.|
|escapeString(sEscapeString)|Escapes the specified string.|
|expectedType()|Returns the type which is expected as a result of the whole template. Makes sense if the template is expanded in the right part of an assignment, after return, etc.|
|fileName(sFileName)|Returns file name with extension.|
|fileNameWithoutExtension()|Returns file name without extension.|
|firstWord(sFirstWord)|返回第一个word|
|groovyScript("groovy code")|Returns Groovy script with the specified code.You can use groovyScript macro with multiple arguments. The first argument is a script text that is executed or a path to the file that contains a script. The next arguments are bound to _1, _2, _3, ..._n variables that are available inside your script. Also, _editor variable is available inside the script. This variable is bound to the current editor.|
|<font color=red>guessElementType (<container>)</font>|返回**集合**中元素类型|
|<font color=red>iterableComponentType(<ArrayOrIterable>)</font>|返回可迭代变量的成员类型|
|<font color=red>iterableVariable()</font>|返回推荐的可迭代类型的变量|
|lineNumber()|返回行号|
|lowercaseAndDash(String)|Returns lower case separated by dashes, of the string passed as a parameter. MyExampleName => my-example-name.|
|methodName()|返回方法名|
|methodParameters()|返回参数列表|
|methodReturnType()|返回返回类型|
|qualifiedClassName()|返回类名全称|
|<font color=red>rightSideType()</font>|返回与右侧表达式相匹配的类型|
|snakeCase(sCamelCaseText)|CamelCase转snake_case|
|spaceSeparated(String)|驼峰转字符串 fooBar=>foo bar.|
|subtypes(sType)|返回子类型|
|<font color=red>suggestIndexName()</font>|返回一个可用下标名i,j|
|<font color=red>suggestVariableName()</font>|返回一个可用的变量名|
|suggestFirstVariableName(sFirstVariableName)|Doesn't suggest true, false, this, super.|
|time(sSystemTime)|返回系统时间|
|typeOfVariable(VAR)|返回变量类型|
|underscoresToCamelCase(sCamelCaseText)|foo_bar=>fooBar|
|underscoresToSpaces(sParameterWithSpaces)|foo_bar=>foo bar|
|user()|返回当前用户名|
|<font color=red>variableOfType(<type>)</font>|返回一个推荐的该类型的变量，类型用全名如"java.util.Collection"|
|JsArrayVariable|返回JavaScript数组名|
|jsClassName()|返回当前js类名|
|jsComponentType|Returns the JavaScript component type.|
|jsMethodName()|返回JavaScript方法名|
|jsQualifiedClassName|返回JavaScript类全名|
|jsSuggestIndexName|JavaScript建议一个下标名|
|jsSuggestVariableName|JavaScript建议一个变量名|
