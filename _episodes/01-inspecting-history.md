  - How can we find out who introduced a line of code and when exactly?
  - Quickly find a line of code, find out who introduced it, when, and why.
$ git show e83c51633
commit e83c5163316f89bfbde7d9ab23ca2e25604af290
Author: Linus Torvalds <torvalds@ppc970.osdl.org>
Date:   Thu Apr 7 15:13:13 2005 -0700
    Initial revision of "git", the information manager from hell
...
diff --git a/README b/README
new file mode 100644
index 000000000..27577f768
--- /dev/null
+++ b/README
@@ -0,0 +1,168 @@
+
+       GIT - the stupid content tracker
+
+"git" can mean anything, depending on your mood.
+
+ - random three-letter combination that is pronounceable, and not
+   actually used by any common UNIX command.  The fact that it is a
+   mispronounciation of "get" may or may not be relevant.
+ - stupid. contemptible and despicable. simple. Take your pick from the
+   dictionary of slang.
+ - "global information tracker": you're in a good mood, and it actually
+   works for you. Angels sing, and a light suddenly fills the room.
+ - "goddamn idiotic truckload of sh*t": when it breaks
+This is a stupid (but extremely fast) directory content manager.  It
+doesn't do a whole lot, but what it _does_ do is track directory
+contents efficiently.
...
Compare this with: [https://github.com/git/git/commit/e83c51633](https://github.com/git/git/commit/e83c51633)
- `git blame` is a fun and useful command to find out when a specific line got introduced and by whom.
```

Example from real life:
```
> *"Who the %&!@!!! wrote this crap?!? Oh, it was me."*
Who was the last to edit a specific line of the source file for `git grep` and when and why?
> *I remember there used to be a line containing the word "great idea".
> Now it is gone:*
What now?
