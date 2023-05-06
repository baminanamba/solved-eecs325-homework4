Download Link: https://assignmentchef.com/product/solved-eecs325-homework4
<br>
<ol>

 <li> Consider the network below. Assume that a simple distance vector routing (without poisoned reverse) is used to route packets.</li>

</ol>

The table below shows the distance and next-hop router to node F from each node after the algorithm stablizes.

<table width="216">

 <tbody>

  <tr>

   <td width="62"> </td>

   <td width="153">Before update (distance, next-hop)</td>

  </tr>

  <tr>

   <td width="62">A to F</td>

   <td width="153">4, E</td>

  </tr>

  <tr>

   <td width="62">B to F</td>

   <td width="153">3, E</td>

  </tr>

  <tr>

   <td width="62">C to F</td>

   <td width="153">4, B</td>

  </tr>

  <tr>

   <td width="62">D to F</td>

   <td width="153">3, F</td>

  </tr>

  <tr>

   <td width="62">E to F</td>

   <td width="153">1, F</td>

  </tr>

 </tbody>

</table>

Assume that routing messages and forwarding table updates happen at the same time on all nodes. Assume routers break ties between equal cost paths by picking the nexthop router with the lower ID.

<ul>

 <li>Using distance vector without Poisoned Reverse, what is E’s second best path to</li>

</ul>

F? (i.e., which one of E’s other neighbors provides the least-cost path to F)

<ul>

 <li>Now the link cost between nodes E and F increases from 1 to 6. Once E detects the change in link cost, what distance to F does E advertise to its neighbors? Fill in the routing entry (distance and next-hop router) that E’s neighbors compute for destination F after receiving E’s update.</li>

</ul>

E’s advertised distance to F is

<table width="216">

 <tbody>

  <tr>

   <td width="62"> </td>

   <td width="153">After E’s update (distance, next-hop)</td>

  </tr>

  <tr>

   <td width="62">A to F</td>

   <td width="153"> </td>

  </tr>

  <tr>

   <td width="62">B to F</td>

   <td width="153"> </td>

  </tr>

  <tr>

   <td width="62">D to F</td>

   <td width="153"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Continuing with the previous question, what distance does B advertise for destination F in the next iteration? Fill in the routing entry (distance and next-hop) that B’s neighbors compute for destination F after receiving B’s update.</li>

</ul>

B’s advertised distance to F is

<table width="216">

 <tbody>

  <tr>

   <td width="62"> </td>

   <td width="153">After B’s update (distance, next-hop)</td>

  </tr>

  <tr>

   <td width="62">A to F</td>

   <td width="153"> </td>

  </tr>

  <tr>

   <td width="62">C to F</td>

   <td width="153"> </td>

  </tr>

  <tr>

   <td width="62">E to F</td>

   <td width="153"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Continuing with the previous question, what distance to F does C now advertise? Fill in the routing entry (distance and next-hop) that C’s neighbors compute for destination F after receiving C’s update.</li>

</ul>

C’s advertised distance to F is

<table width="215">

 <tbody>

  <tr>

   <td width="61"> </td>

   <td width="153">After C’s update (distance, next-hop)</td>

  </tr>

  <tr>

   <td width="61">B to F</td>

   <td width="153"> </td>

  </tr>

 </tbody>

</table>

Are all routers now following the correct shortest path?                 Yes               No

<ul>

 <li>Will the routing tables converge faster if we use Poisoned Reverse?</li>

</ul>

<ol start="2">

 <li>(8pts) <strong>General Routing. </strong>Consider the network shown below. Supporse AS3 and AS2 are running OSPF for their intra-AS routing protocol. Suppose AS1 and AS4 aer running RIP (distance vector routing algorithm) for their intra-AS routing protocol. Supppose eBGP and iBGP are used for the inter-AS routing protocol. Initially suppose there is <em>no </em>physical link between AS2 and AS4.</li>

</ol>

a Router 3c learns about prefix x from which routing protocol: OSPF, RIP, eBGP, or iBGP? b Router 3a learns about x from which routing protocol? c Router 1c learns about x from which routing protocol?

d Router 1d learns about x from which routing protocol?

<strong>BGP Policies. </strong>Consider an interdomain network with domains A through F. For simplicity, assume that destination in this problem are domains, not prefixes. Routes are represented by a series of domains, e.g., [A – B – C] denotes a route that start with domain A and go to domain B and then go to domain C (which is the destination). Domains always advertise the route to themselves (i.e., domain X advertise paths to X to all peers, customers, and providers). The following connectivity/business relationship exists:

<ul>

 <li>B is a customer of A</li>

 <li>C is a customer of A</li>

 <li>D is a customer of A</li>

 <li>B and C are peers</li>

 <li>C and D are peers</li>

 <li>E is a customer of B</li>

 <li>F is a customer of B</li>

 <li>F is a customer of C</li>

 <li>G is a customer of D</li>

</ul>

Assuming that each domain’s routing policies follow normal business practice, and that

BGP has converged,

<ol>

 <li>i) What routes does A advertise to B? ii) What routes does C advertise to B? iii) What routes does E advertise to B? iv) What routes does F advertise to B?</li>

</ol>