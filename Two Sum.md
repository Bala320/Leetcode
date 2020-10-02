<ol>
<li class="has-line-data" data-line-start="0" data-line-end="7">Two Sum<br>
Easy<br>
16648602Add to ListShare<br>
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.<br>
You may assume that each input would have exactly one solution, and you may not use the same element twice.<br>
You can return the answer in any order.</li>
</ol>
<p class="has-line-data" data-line-start="7" data-line-end="17">Example 1:<br>
Input: nums = [2,7,11,15], target = 9<br>
Output: [0,1]<br>
Output: Because nums[0] + nums[1] == 9, we return [0, 1].<br>
Example 2:<br>
Input: nums = [3,2,4], target = 6<br>
Output: [1,2]<br>
Example 3:<br>
Input: nums = [3,3], target = 6<br>
Output: [0,1]</p>
<p class="has-line-data" data-line-start="18" data-line-end="27">Constraints:<br>
•   2 &lt;= nums.length &lt;= 105<br>
•   -109 &lt;= nums[i] &lt;= 109<br>
•   -109 &lt;= target &lt;= 109<br>
•   Only one valid answer exists.<br>
Accepted<br>
3.3M<br>
Submissions<br>
7.1M</p>
<p class="has-line-data" data-line-start="30" data-line-end="47">CODE—&gt;&gt;&gt;&gt;&gt;<br>
class Solution<br>
{<br>
public int[] twoSum(int[] nums, int target)<br>
{    int a[]=new int[2];<br>
for(int i=0;i&lt;nums.length;i++)<br>
{<br>
for(int j=i+1;j&lt;nums.length;j++)<br>
{<br>
if(nums[j]+nums[i]==target)<br>
{<br>
a[0]=i;<br>
a[1]=j;<br>
return a;<br>
}<br>
}<br>
}</p>
<pre><code>   throw new IllegalArgumentException(&quot;No two sum solution&quot;);
</code></pre>
<p class="has-line-data" data-line-start="50" data-line-end="52">}<br>
}</p>
