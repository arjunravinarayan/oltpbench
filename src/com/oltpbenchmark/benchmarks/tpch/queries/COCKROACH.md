TPC-H on cockroach
===
Legend:
  #: Modifications made to get the query to work
  !!!: queries that don't work pending features.


* table creation works fine
* index creation works fine
* query1 #
    * interval +/- dates not supported (#12416). Tweaked.
    * '95' day not supported. Change to '95 day'. Tweaked.
* query2 !!!
    * nested query access of outer query's columns (#7042)
* query3
    * works fine.
* query4 !!!
    * #7042
* query5 !!!
    * #12416. Tweaked.
    * #7042
* query6
    * works fine.
* query7 #
    * #12416. Tweaked.
* query8 #
    * #12416. Tweaked.
* query9 #
    * #12416. Tweaked.
* query10
    * #12416. Tweaked.
* query11
    * works fine
* query12 #
    * #12416. Tweaked.
* query13
    * works fine
* query14 #
    * #12416. Tweaked.
* query15-create-view #
    * #12416. Tweaked.
    * '3' month -> '3 month. Tweaked.
* query15 !!!
    * #12420. VIEWs are buggy. Pending fix.
* query16
    * works fine
* query17 !!!
    * #7042
* query18
    * works fine
* query19
    * works fine
* query20 !!!
    * #7042? Not sure
* query21 !!!
    * ???
* query22 !!!
    * #7042.
