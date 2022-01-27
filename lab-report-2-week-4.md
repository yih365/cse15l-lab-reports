
1) testFile2(MarkdownParseTest)
java.io.IOException
        at MarkdownParse.getLinks(MarkdownParse.java:27)
        at MarkdownParseTest.testFile2(MarkdownParseTest.java:32)


1) testFile3(MarkdownParseTest)
java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 31      
        at java.base/java.lang.String.checkBoundsBeginEnd(String.java:3751)
        at java.base/java.lang.String.substring(String.java:1907)
        at MarkdownParse.getLinks(MarkdownParse.java:25)
        at MarkdownParseTest.testFile3(MarkdownParseTest.java:40)
2) testFile4(MarkdownParseTest)
java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 28
        at java.base/java.lang.String.checkBoundsBeginEnd(String.java:3751)
        at java.base/java.lang.String.substring(String.java:1907)
        at MarkdownParse.getLinks(MarkdownParse.java:25)
        at MarkdownParseTest.testFile4(MarkdownParseTest.java:48)
