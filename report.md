<h1>Clustering US states and territories for fair distribution of US education budget among the states</h1>

<h3 style = "color: 'blue';">Introduction</h3>
<p>
  Let us suppose that the US government wants to classify it's states into three tiers so that it can distribute its education budget
  among the states in such a manner that the ones belonging to the third tier (having less educational development) get larger share, and the ones belonging
  to the first tier (having more educational development) get smaller share.
  <br>
  Basically, the task here is to divide the states into three clusters. 
  <ul>
      <li>Tier 1: More Educationally Developed</li>
      <li>Tier 2: Moderately Educationally Developed</li>
      <li>Tier 3: Less Educationally Developed</li>
  </ul>
  One very important question arises here. <br/><br/>
  <b> How can one measure the educational development of a state?</b>
  <br/>
</p>
<h3 style = "color: 'blue';">Data </h3>
<p>
  Let's talk about the 'search' endpoint of Foresquare API. One cool thing about it is that if you enter a word in the query when you use
  this end point, the Foresquare API, behind the scene, searches not for the query word you mentioned but also for similar words.
  <br/><br/>
  Let us assume here that the educational development can be measured by the number of educational institutions. The more the educational institutions
  a state has, the more it is educatationally developed.
  <br/><br/>
  And the best thing about the Foursquare API is that if you search for school, it will return results of schools, colleges, universities, etc.
  <br/><br/>
  So, now we can us the Foresquare API to extract the information of the educational institutes for each state. Since we have to apply clustering on the states,
  we will try to keep the educational institutions into various categories, e.g. number of primary schools, number of secondary schools, universities, etc.
  We can then apply clustering on the states to divide them into three clusters. And, finally we will try to see whether the literacy data 
  ( literacy data for each of the states) justifies the results of clustering. Through the same data, we will deduce which clusters 
  should be labelled as <i>tier 1</i>, <i>tier 2</i>, and <i>tier 3</i>.
  <br/><br/>
  The literacy data can be extracted from the Wikipedia.
</p>
