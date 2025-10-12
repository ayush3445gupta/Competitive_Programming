<h3><a href="https://codeforces.com/contest/1693/problem/A" target="_blank" rel="noopener noreferrer">Directional Increase</a></h3>

<div class="header"><div class="title">A. Directional Increase</div><div class="time-limit"><div class="property-title">time limit per test</div>1 second</div><div class="memory-limit"><div class="property-title">memory limit per test</div>256 megabytes</div><div class="input-file input-standard"><div class="property-title">input</div>standard input</div><div class="output-file output-standard"><div class="property-title">output</div>standard output</div></div><div><p>We have an array of length $$$n$$$. Initially, each element is equal to $$$0$$$ and there is a pointer located on the first element.</p><p>We can do the following two kinds of operations any number of times (possibly zero) in any order:</p><ol><li> If the pointer is not on the last element, increase the element the pointer is currently on by $$$1$$$. Then move it to the next element.</li><li> If the pointer is not on the first element, decrease the element the pointer is currently on by $$$1$$$. Then move it to the previous element.</li></ol><p>But there is one additional rule. <span class="tex-font-style-bf">After we are done, the pointer has to be on the first element.</span></p><p>You are given an array $$$a$$$. Determine whether it's possible to obtain $$$a$$$ after some operations or not.</p></div><div class="input-specification"><div class="section-title">Input</div><p>The first line contains a single integer $$$t$$$ $$$(1\le t\le 1000)$$$  — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $$$n$$$ $$$(1\le n\le 2 \cdot 10^5)$$$  — the size of array $$$a$$$.</p><p>The second line of each test case contains $$$n$$$ integers $$$a_1, a_2, \ldots, a_n$$$ ($$$-10^9 \le a_i \le 10^9$$$) — elements of the array.</p><p>It is guaranteed that the sum of $$$n$$$ over all test cases doesn't exceed $$$2 \cdot 10^5$$$.</p></div><div class="output-specification"><div class="section-title">Output</div><p>For each test case, print "Yes" (without quotes) if it's possible to obtain $$$a$$$ after some operations, and "No" (without quotes) otherwise.</p><p>You can output "Yes" and "No" in any case (for example, strings "yEs", "yes" and "Yes" will be recognized as a positive response).</p></div><div class="sample-tests"><div class="section-title">Example</div><div class="sample-test"><div class="input"><div class="title">Input<div title="Copy" data-clipboard-target="#id007011384219423988" id="id008126738301550013" class="input-output-copier">Copy</div></div><pre id="id007011384219423988">7
2
1 0
4
2 -1 -1 0
4
1 -4 3 0
4
1 -1 1 -1
5
1 2 3 4 -10
7
2 -1 1 -2 0 0 0
1
0
</pre></div><div class="output"><div class="title">Output<div title="Copy" data-clipboard-target="#id0007930355855870452" id="id0030418056696542606" class="input-output-copier">Copy</div></div><pre id="id0007930355855870452">No
Yes
No
No
Yes
Yes
Yes
</pre></div></div></div><div class="note"><div class="section-title">Note</div><p>In the first test case we can obtain the array after some operations, but the pointer won't be on the first element.</p><p>One way of obtaining the array in the second test case is shown below.</p><p>$$$\langle \underline{0}, 0, 0, 0\rangle \to \langle 1, \underline{0}, 0, 0 \rangle \to \langle \underline{1}, -1, 0, 0\rangle \to \langle 2, \underline{-1}, 0, 0\rangle \to \langle 2, 0, \underline{0}, 0\rangle \to \langle 2, \underline{0}, -1, 0\rangle \to \langle \underline{2}, -1, -1, 0\rangle$$$</p></div>