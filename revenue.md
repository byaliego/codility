<p>A company has a list of expected revenues and payments for the upcoming year in chronological order. The problem is that at some moments in time the sum of previous payments can be larger than the total previous revenue. This would put the company in debt. To avoid this problem the company takes a very simple approach. It reschedules some expenses to the end of the year.</p>
<p>You are given an array of integers, where positive numbers represent revenues and negative numbers represent expenses, all in chronological order. In one move you can relocate any expense (negative number) to the end of the array. What is the minimum number of such relocations to make sure that the company never falls into debt? In other words: you need to make sure that there is no consecutive sequence of elements starting from the beginning of the array, that sums up to a negative number.</p>
<p>You can assume that the sum of all elements in A is nonnegative.</p>
<p>Write a function:</p>
<blockquote><p style="font-family: monospace; font-size: 9pt; display: block; white-space: pre-wrap"><tt>class Solution { public int solution(int[] A); }</tt></p></blockquote>
<p>that, given an array A of N integers, returns the minimum number of relocations, so that company never falls into debt.</p>
<p><b>Examples:</b></p>
<p>1. Given A = [10, -10, -1, -1, 10], the function should return 1. It is enough to move -10 to the end of the array.</p>
<p>2. Given A = [-1, -1, -1, 1, 1, 1, 1], the function should return 3. The negative elements at the beginning must be moved to the end to avoid debt at the start of the year.</p>
<p>3. Given A = [5, -2, -3, 1], the function should return 0. The company balance is always nonnegative.</p>
<p>Write an <b><b>efficient</b></b> algorithm for the following assumptions:</p>
<blockquote><ul style="margin: 10px;padding: 0px;"><li>N is an integer within the range [<span class="number">1</span>..<span class="number">100,000</span>];</li>
<li>each element of array A is an integer within the range [<span class="number">−1,000,000,000</span>..<span class="number">1,000,000,000</span>];</li>
<li>sum of all elements in A is greater than or equal to 0.</li>
</ul>
</blockquote>
