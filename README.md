# IDEA_BUG_REPORT

1.Please open this as a project.
2.Open src/MAINCLASS and delete all '/', '/*', '*/'.
3.Build the project and run MAINCLASS, you will see a file named TEST.class in out/production/BUG_TEST, open this and be attention to the file name and the case of the content.
4.Open src/testclass and delete all '/', '/*', '*/'.
5.Build the project, and open TEST.class mentioned in 3.
6.Look at the content of that file, you will find that it has been rewritten.
7.Open src/MAINCLASS and run, you will find an error "ClassNotFound" is raised.

Overall, I think IDEA shouldn't allow users to create enums or some other data structures which will be generated automatically in the out filter with the same spellation and different case. Because Windows is not sensitive to the case of the file name.
