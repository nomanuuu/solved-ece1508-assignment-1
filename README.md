Download Link: https://assignmentchef.com/product/solved-ece1508-assignment-1
<br>
<h1></h1>

<ul>

 <li>Create the network topology using <strong>mininet’s </strong>command line options<strong>. </strong>Do not add any controller for path setup.</li>

 <li>Use <strong>ovs-ofctl</strong> to create two bidirectional paths, <em>e.</em>, the <strong>orange</strong> path between <strong>h1 </strong>and <strong>h9 </strong>and the  <strong>purple</strong> path between <strong>h3 </strong>and <strong>h7</strong>. (no other pair of hosts should be able to communicate).</li>

 <li>After setting up the path run the following from mininet console:

  <ul>

   <li><strong>iperf h1 h9</strong></li>

  </ul></li>

</ul>

<strong>○ </strong><strong>iperf h3 h7 </strong>● Then run <strong>h1 ping h9    </strong>Link bandwidth = 15Mbps

Link delay = 10ms

<strong>Tips/Resources</strong>

<ul>

 <li>Run mininet with <strong>–arp</strong> option to statically populate arp table in the hosts. A reference for example <strong>ovs-ofctl add-flow</strong>:

  <ul>

   <li><u>https://docs.pica8.com/pages/viewpage.action?pageId=3086345</u> Set an <strong>idle_timeout</strong> of <strong>0</strong> so that flows do not expire.</li>

  </ul></li>

</ul>

<strong>What to submit?</strong>

<table width="864">

 <tbody>

  <tr>

   <td width="57">●</td>

   <td colspan="2" width="807">Put the following files inside a compressed folder named<strong>&lt;lastname_firstname_university.zip&gt;</strong> where university is one of <strong>waterloo, toronto, laval, ets</strong></td>

  </tr>

  <tr>

   <td width="57">●</td>

   <td width="720"><strong>command.sh</strong> — File containing the command to create the topology</td>

   <td width="87">         <strong>(10)</strong></td>

  </tr>

  <tr>

   <td width="57">●</td>

   <td width="720">Files created by the following commands (after path setup):○ <strong>ovs-ofctl dump-flows s1 &amp;&gt; s1                          </strong><strong>        </strong></td>

   <td width="87"><strong>         (5)</strong></td>

  </tr>

  <tr>

   <td width="57"></td>

   <td width="720"><strong>○ </strong><strong>ovs-ofctl dump-flows s2 &amp;&gt; s2                          </strong><strong>        </strong></td>

   <td width="87"><strong>(5)</strong></td>

  </tr>

  <tr>

   <td width="57"></td>

   <td width="720"><strong>○ </strong><strong>ovs-ofctl dump-flows s4 &amp;&gt; s4                          </strong><strong>        </strong></td>

   <td width="87"><strong>(5)</strong></td>

  </tr>

  <tr>

   <td width="57">●</td>

   <td width="720">Output of <strong>iperf </strong>commands○ Filename: iperf.out○ One line for each iperf output in the following format: ■ &lt;host_id&gt; — &lt;host_id&gt;: &lt;reported_bw&gt;</td>

   <td width="87">         <strong>(10)</strong></td>

  </tr>

  <tr>

   <td width="57">●</td>

   <td width="720">Average of the first 5 reported round trip times from ping output.○ Filename: <strong>latency.out</strong>○ One line containing the average round trip time</td>

   <td width="87"><strong>(5)</strong></td>

  </tr>

 </tbody>

</table>





