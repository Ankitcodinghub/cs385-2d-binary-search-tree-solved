# cs385-2d-binary-search-tree-solved
**TO GET THIS SOLUTION VISIT:** [CS385 2D Binary Search Tree Solved](https://www.ankitcodinghub.com/product/cs385-2d-binary-search-tree-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;36125&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS385 2D Binary Search Tree Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
A 2D tree is a binary search tree in which each node contains a 2D point and holds the x and y coordinates of that node. 2D tree generalizes a binary search tree in that it positions each node according to either the x or y coordinates of its data point. The coordinate choice depends on the level at which the node is added into the tree. The first point you add into an empty tree is placed into a node that becomes the tree’s root. IF the next point to be added has an x-coordinate that is less than the x-coordinate of the point in the root, you place the new point into the left child of the root. Otherwise, you place it into root’s right child. Insertions at the next level—level 3—compares y-coordinates; insertion at level 4 compares x-coordinates, and so on.

For example, suppose we want to add the points (50,40),(40,70),(80,20),(90,10), and (60,30) into an initially empty 2d tree ( the process is illustrated below)

<ul>
<li>The first point becomes the root node</li>
<li>To add (40,70), you compare 40, the point’s x-coordinate, with 50, the x-coordinate of the root. Since 40 is less than 50, you move to the left. The left child of root is null so the new point goes into the left child of the root.</li>
<li>To add (80,20), you compare 80 with 50, the x-coordinates of the root node. Since 80 is greater than 50, you move to the right. The right child of the root is null, so new node (80,50) is placed in to the right child of the root.</li>
<li>To add the next point, (90,10), you compare 90 with the x-coordinate of the root node. 90 is greater than 50, so you move to the right child and compare the y-coordinate with the right child. 10 is less than 20, the y-coordinate of the root’s right child. Hence, you move to the left. The left child of (80,20) is null, hence, the new node (90,10) is added as the left child of (80,20)</li>
<li>To add the next point (60,8), you compare 60 with x-coordinate of the root. 60 is greater than</li>
</ul>
50, so you move to the right. Then you compare the y coordinates of (60,8) with y-coordinate of (80,20). 8&lt;20 so you move to the left. Then you compare the x coordinate of (60,8) with the x coordinate of (90,10); 60&lt;90 so you move to the left. The left child of (90,10) is null, so you place (60,8) to the left of (90,10)..

In summary, to insert a new node into a 2d-tree you keep searching in the binary tree switching between x and y coordinates at each level until you hit a null node and you insert the new node there.

The file TwoDTree.java attached to this assignment provides a skeleton for implementation of a 2-d tree. This file contains a nested class TwoDTreeNode which represents a node in the TwoDTree and holds the x and y coordinates for the node as well as references to its left and right children.

Your job is to implement two methods in this file:

<ol>
<li><strong>Public void add( int x, int y) :</strong> This method adds a new node with coordinates (x,y) to the 2d tree. Duplicate nodes are not allowed in the tree.</li>
<li><strong>public boolean contains(int x, int y): </strong>This method returns true if a node with given x and y coordinates exist in the TwoDTree.</li>
</ol>
I have also provided a helper method levelOrderPrint to print the level-order traversal of the tree. This method helps you test your add method and view a level order traversal of the tree after adding nodes to it.&nbsp; You can use any additional helper method you want.

<strong>Hints:&nbsp; </strong>

<ul>
<li>For implementing the add method, you can use the add(T obj) method in the</li>
</ul>
GenericBinarySearchTree .java file (provided under “source code” section on blackboard) as an example and modify it to fit the specification of this problem.&nbsp; For example, to find the insertion point for a new node, you start from the root node and go down the tree. At each point you decide to go left or right based on comparing the current node with x or y coordinate. The choice of which coordinate to use depends on the level in which you are performing the comparison.&nbsp; At root level (level 0) the x coordinate is used for comparison; at next level (level 1) the y coordinate is used for comparison, at level 2, the x coordinate is used for comparison, and so on.

<ul>
<li>Once you implement the add method, the contain method should be easy to implement. You simply follow the same process. To find a given node, you start at the root node and go down the tree to find the node. At each point you compare the x or y coordinate with the current node and decide to go left or right. The choice of coordinate depends on the level on which you are doing the comparison.</li>
<li>Please make sure to test your method for various test cases. I made up a small sample main method. The main method and the result of its run is shown below:</li>
</ul>
<strong>&nbsp;</strong>

&nbsp;

&nbsp;

&nbsp;
