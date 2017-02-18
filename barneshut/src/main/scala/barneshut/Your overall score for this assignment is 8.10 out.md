Your overall score for this assignment is 8.10 out of 10.00


The code you submitted did not pass all of our tests: your submission achieved a score of
8.10 out of 10.00 in our tests.

In order to find bugs in your code, we advise to perform the following steps:
 - Take a close look at the test output that you can find below: it should point you to
   the part of your code that has bugs.
 - Run the tests that we provide with the handout on your code.
 - The tests we provide do not test your code in depth: they are very incomplete. In order
   to test more aspects of your code, write your own unit tests.
 - Take another very careful look at the assignment description. Try to find out if you
   misunderstood parts of it. While reading through the assignment, write more tests.

Below you can find a short feedback for every individual test that failed.

======== LOG OF FAILED TESTS ========
Your solution achieved a testing score of 51 out of 63.

Below you can see a short feedback for every test that failed,
indicating the reason for the test failure and how many points
you lost for each individual test.

Tests that were aborted took too long too complete or crashed the
JVM. Such crashes can arise due to infinite non-terminitaing
loops or recursion (StackOverflowException) or excessive memory
consumption (OutOfMemoryException).

[Test Description] Fork with 4 empty quadrants
[Observed Error] NaN did not equal 20.0 NaN should be 20f
[Lost Points] 2

[Test Description] Body.updated should consider a Fork as opaque if it is far away
[Observed Error] 0.84799826 was not less than 0.5 Sanity check: the fork is indeed far enough
[Lost Points] 2

[Test Description] Leaf.insert(b) should return a new Fork if size > minimumSize
[Observed Error] List(false, false, false, false) (of class scala.collection.immutable.$colon$colon)
[exception was thrown] detailed error message in debug output section below
[Lost Points] 2

[Test Description] Fork.insert(b) should insert recursively in the appropriate quadrant
[Observed Error] Fork(Leaf(10.0,30.0,10.0,List(barneshut.package$Body@72f926e6)),Leaf(20.0,30.0,10.0,List(barneshut.package$Body@3daa422a)),Empty(10.0,40.0,10.0),Leaf(20.0,40.0,10.0,List(barneshut.package$Body@31c88ec8))) should be a Fork where only ne changed
[Lost Points] 2

[Test Description] 'insert' should work correctly on a leaf with center (1,1) and size 2
[Observed Error] Fork(Fork(Leaf(0.25,0.25,0.5,List(barneshut.package$Body@3d51f06e)),Leaf(0.75,0.25,0.5,List(barneshut.package$Body@7ed7259e)),Empty(0.25,0.75,0.5),Empty(0.75,0.75,0.5)),Empty(1.5,0.5,1.0),Empty(0.5,1.5,1.0),Empty(1.5,1.5,1.0)) did not equal Fork(Leaf(0.5,0.5,1.0,List(barneshut.package$Body@3d51f06e)),Leaf(1.5,0.5,1.0,List(barneshut.package$Body@7ed7259e)),Empty(0.5,1.5,1.0),Empty(1.5,1.5,1.0)) expected Fork(Leaf(0.5,0.5,1.0,List(barneshut.package$Body@3d51f06e)),Leaf(1.5,0.5,1.0,List(barneshut.package$Body@7ed7259e)),Empty(0.5,1.5,1.0),Empty(1.5,1.5,1.0)) found Fork(Fork(Leaf(0.25,0.25,0.5,List(barneshut.package$Body@3d51f06e)),Leaf(0.75,0.25,0.5,List(barneshut.package$Body@7ed7259e)),Empty(0.25,0.75,0.5),Empty(0.75,0.75,0.5)),Empty(1.5,0.5,1.0),Empty(0.5,1.5,1.0),Empty(1.5,1.5,1.0))
[Lost Points] 2

[Test Description] Body.updated should recursively traverse a Fork close to it
[Observed Error] FloatOps.DoubleOps(body.xspeed.toDouble).~=(0.2641816735267639) was false xspeed was 0.0
[Lost Points] 2

======== TESTING ENVIRONMENT ========
Limits: memory: 256m,  total time: 850s,  per test case time: 240s

======== DEBUG OUTPUT OF TESTING TOOL ========
matrix: 106 ms; avg: NaN
matrix: 3 ms; avg: NaN
matrix: 3 ms; avg: NaN
update: 10 ms; avg: NaN
update: 1 ms; avg: NaN
[test failure log] test name: BarnesHutSuite::Leaf.insert(b) should return a new Fork if size > minimumSize::2
scala.MatchError: List(false, false, false, false) (of class scala.collection.immutable.$colon$colon)
barneshut.package$Fork.insert(package.scala:71)
barneshut.package$Leaf$$anonfun$insert$1.apply(package.scala:88)
barneshut.package$Leaf$$anonfun$insert$1.apply(package.scala:88)
scala.collection.LinearSeqOptimized$class.foldLeft(LinearSeqOptimized.scala:124)
scala.collection.immutable.List.foldLeft(List.scala:84)
barneshut.package$Leaf.insert(package.scala:88)
barneshut.package$Fork.insert(package.scala:72)
barneshut.package$Leaf$$anonfun$insert$1.apply(package.scala:88)
barneshut.package$Leaf$$anonfun$insert$1.apply(package.scala:88)
scala.collection.LinearSeqOptimized$class.foldLeft(LinearSeqOptimized.scala:124)
scala.collection.immutable.List.foldLeft(List.scala:84)
barneshut.package$Leaf.insert(package.scala:88)
barneshut.BarnesHutSuite$$anonfun$14.apply$mcV$sp(BarnesHutSuite.scala:234)
ch.epfl.lamp.grading.GradingSuite$$anonfun$test$1.apply$mcV$sp(GradingSuite.scala:118)
ch.epfl.lamp.grading.GradingSuite$$anonfun$test$1.apply(GradingSuite.scala:117)
ch.epfl.lamp.grading.GradingSuite$$anonfun$test$1.apply(GradingSuite.scala:117)
org.scalatest.Transformer$$anonfun$apply$1.apply$mcV$sp(Transformer.scala:22)
org.scalatest.OutcomeOf$class.outcomeOf(OutcomeOf.scala:85)
org.scalatest.OutcomeOf$.outcomeOf(OutcomeOf.scala:104)
org.scalatest.Transformer.apply(Transformer.scala:22)
org.scalatest.Transformer.apply(Transformer.scala:20)
org.scalatest.FunSuiteLike$$anon$1.apply(FunSuiteLike.scala:166)
org.scalatest.Suite$class.withFixture(Suite.scala:1122)
org.scalatest.FunSuite.withFixture(FunSuite.scala:1555)
org.scalatest.FunSuiteLike$class.invokeWithFixture$1(FunSuiteLike.scala:163)