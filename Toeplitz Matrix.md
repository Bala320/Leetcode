<ol start="766">
<li class="has-line-data" data-line-start="0" data-line-end="3">Toeplitz Matrix<br>
Easy</li>
</ol>
<p class="has-line-data" data-line-start="3" data-line-end="4">1146</p>
<p class="has-line-data" data-line-start="5" data-line-end="6">83</p>
<p class="has-line-data" data-line-start="7" data-line-end="8">Add to List</p>
<p class="has-line-data" data-line-start="9" data-line-end="11">Share<br>
A matrix is Toeplitz if every diagonal from top-left to bottom-right has the same element.</p>
<p class="has-line-data" data-line-start="12" data-line-end="13">Now given an M x N matrix, return True if and only if the matrix is Toeplitz.</p>
<p class="has-line-data" data-line-start="15" data-line-end="16">Example 1:</p>
<p class="has-line-data" data-line-start="17" data-line-end="29">Input:<br>
matrix = [<br>
[1,2,3,4],<br>
[5,1,2,3],<br>
[9,5,1,2]<br>
]<br>
Output: True<br>
Explanation:<br>
In the above grid, the diagonals are:<br>
“[9]”, “[5, 5]”, “[1, 1, 1]”, “[2, 2, 2]”, “[3, 3]”, “[4]”.<br>
In each diagonal all elements are the same, so the answer is True.<br>
Example 2:</p>
<p class="has-line-data" data-line-start="30" data-line-end="38">Input:<br>
matrix = [<br>
[1,2],<br>
[2,2]<br>
]<br>
Output: False<br>
Explanation:<br>
The diagonal “[1, 2]” has different elements.</p>
<p class="has-line-data" data-line-start="39" data-line-end="40">Note:</p>
<p class="has-line-data" data-line-start="41" data-line-end="44">matrix will be a 2D array of integers.<br>
matrix will have a number of rows and columns in range [1, 20].<br>
matrix[i][j] will be integers in range [0, 99].</p>
<p class="has-line-data" data-line-start="45" data-line-end="46">Follow up:</p>
<p class="has-line-data" data-line-start="47" data-line-end="49">What if the matrix is stored on disk, and the memory is limited such that you can only load at most one row of the matrix into the memory at once?<br>
What if the matrix is so large that you can only load up a partial row into the memory at once?</p>
<p class="has-line-data" data-line-start="52" data-line-end="67">CODE- java<br>
class Solution {<br>
public boolean isToeplitzMatrix(int[][] n)<br>
{<br>
for(int i=0;i&lt;n.length-1;i++)<br>
{<br>
for(int j=0;j&lt;n[0].length-1;j++)<br>
{<br>
if(n[i][j]!=n[i+1][j+1])<br>
return false;<br>
}<br>
}<br>
return true;<br>
}<br>
}</p>
