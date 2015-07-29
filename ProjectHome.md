## WARNING: QueryReview is now maintained by a new owner.  It is (of course) on github now: ##
https://github.com/nesquena/query_reviewer


This rails plugin not only runs "EXPLAIN" before each of your select queries in development, but provides a small DIV in the rendered output of each page with the summary of query warnings that it analyzed.

It provides the following features:
  * View all EXPLAIN output for all SELECT queries to generate a page (everything that query\_analyzer plugin does)
  * View SHOW PROFILE ALL output for queries that take significant time
  * Rate a page's SQL usage into one of three categories: OK, WARNING, CRITICAL
  * Display the number of SELECT, INSERT, UPDATE, and DELETE queries on each page
  * Attach meaningful warnings to individual queries
  * Provide smart ruby stack traces for each query
  * Display interactive summary on page in development modes
  * Aggregate near-identical queries and find out their total cost

Developed by [Kongregate](http://www.kongregate.com) and [David Stevenson](http://flouri.sh), with additional support from Kevin Hall.

**To install:**

git clone git://github.com/dsboulder/query\_reviewer.git vendor/plugins/query\_reviewer

OR if necessary (I'm NOT 100% committing to keeping the SVN up to date):

svn export http://query-reviewer.googlecode.com/svn/trunk/ vendor/plugins/query\_reviewer

_Tested under rails 2.1, 2.0, and 1.2.3_

**Want to see what it looks like?**

http://flouri.sh/2008/4/10/mysql-query-reviewer-now-with-ajax-and-profiling

http://flouri.sh/2008/2/13/mysql-query_reviewer-plugin

http://flouri.sh/2008/9/10/queryreviewer-now-aggregates-identical-queries