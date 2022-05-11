<ul>
<li>SHA-2 includes significant changes from its predecessor, SHA-1.</li>
<li>The SHA-2 family consists of six hash functions with digests (hash values) that are 224, 256, 384 or 512 bits;
  SHA-224, SHA-256, SHA-384, SHA-512, SHA-512/224, SHA-512/256.</li>
<li>SHA-256 and SHA-512 are novel hash functions computed with eight 32-bit and 64-bit words, respectively. They use different shift amounts and additive constants, but their structures are otherwise virtually identical, differing only in the number of rounds.</li>
<li>SHA-224 and SHA-384 are truncated versions of SHA-256 and SHA-512 respectively, computed with different initial values.</li>
<li>SHA-512/224 and SHA-512/256 are also truncated versions of SHA-512, but the initial values are generated using the method described in Federal Information Processing Standards (FIPS) PUB 180-4.</li></ul>
<hr size="8" width="100%" color="black">  

  <u>SHA-224 is identical to SHA-256, except that:</u>
<ul>
<li>the initial hash values h0 through h7 are different, and the output is constructed by omitting h7.</li>
</ul>


<u>SHA-512 is identical in structure to SHA-256, but:</u>
<ul>
  <li>the message is broken into 1024-bit chunks</li>
<li>the initial hash values and round constants are extended to 64 bits</li>
<li>there are 80 rounds instead of 64</li>
<li>the message schedule array w has 80 64-bit words instead of 64 32-bit words</li>
<li>to extend the message schedule array w, the loop is from 16 to 79 instead of from 16 to 63</li>
<li>the round constants are based on the first 80 primes 2..409</li>
<li>the word size used for calculations is 64 bits long</li>
<li>the appended length of the message (before pre-processing), in bits, is a 128-bit big-endian integer, and</li>
<li>the shift and rotate amounts used are different.</li>
  </ul>
  
  <u>SHA-512/t is identical to SHA-512 except that:</u>
<ul>
<li>the initial hash values h0 through h7 are given by the SHA-512/t IV generation function,</li>
<li>the output is constructed by truncating the concatenation of h0 through h7 at t bits,</li>
<li>t equal to 384 is not allowed, instead SHA-384 should be used as specified, and</li>
<li>t values 224 and 256 are especially mentioned as approved.</li>
</ul>


<html>
<body>
  
<h2>Comparison of SHA-2 functions</h2>

<table style="width:100%">
  <tbody>
  <tr>
<th rowspan="2">Algorithm and variant</th>
<th rowspan="2">Output size<br />(bits)</th>
<th rowspan="2">Internal <br />state size <br />(bits)</th>
<th rowspan="2">Block size<br />(bits)</th>
<th rowspan="2">Rounds</th>
  </tr>
  <tr>
<td><i>SHA-224</i><br /><i>SHA-256</i></td>
<td>224<br />256</td>
<td>256<br /></td>
<td>512</td>
<td>64</td>
  </tr>
</tbody></table>
</body>
</html>

<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
}
</style>
<body>

<h2>A basic HTML table</h2>

<table style="width:100%">
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>

<p>To undestand the example better, we have added borders to the table.</p>

</body>
</html>


