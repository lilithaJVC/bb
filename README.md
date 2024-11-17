<ol>welcome  to the municipal  application, this is the third and the final part of this application </ol>
<ol>functional requirements </ol>

<ol>How to complite an application </ol>

<li>make sure you have visual studio installed into your device</li>
<li>get acess to my git hub repository </li>
<li>clone the repository using the link  </li>
<li>when the  application launches it will   take users to the home page that have 3 menu items </li>
<li>these methu items consist of report issue , load events and announcements as well as service request status  </li>
<li>when the user clicks the service request status button from the menu itemit will load all the submitted service requests including their status </li>
<li>the user is able to submit new service request by providing the service request unique number /li>
<li>the description as well as the status of that service request </li>
<li>users are also able to track the status of their service request by providing the identifier of that service request by searching them </li>
                                    
<ol>The structures that I used are Binary search tree and Mini-Heap</ol>

<li></li>Binary Search Tree (BST)<li></li>
<li>Role: The BST helps store and manage the Service Request Model objects. It helps to organize the requests by their RequestID, this makes it efficient to search for specific requests based on their ID. The key idea behind the BST is that for each node, all elements in the left subtree are smaller, and all elements in the right subtree are greater. This structure ensures that the searching operation that is finding a request by its ID, happens in O (log n) time complexity, where n is the number of requests in the tree.
</li>	
<ol></ol>	Efficiency Contribution:</ol>

<li>Searching: this helps to quickly find any service using the RequestID by using the Search method. Instead of searching through all the requests sequentially, the BST allows you directly jump to the correct node, drastically improving search time.</li>
<li></li>	Example: If a user wants to track a specific service request (for example they want to search for RequestID number 3), the BST will efficiently locate that request, and return its details (Description as well as their Status) without having to search through all requests</li>
<li>In-Order Traversal: The BST can also be traversed in in-order to retrieve all the requests in ascending order of RequestID. This ensures that the requests are displayed in a sorted manner in the UI.
Min-Heap</li>
<li>	Role: The Min-Heap is used to manage the priority of service requests. It is used to store requests based on their Priority level, where the highest-priority request (lowest priority number) is always at the root. A Min-Heap ensures that when you need to retrieve or process the highest-priority request, it can be done in O (log n) time.
Efficiency Contribution:</li>
<li>	Priority Management: The service requests are inserted into the Min-Heap with their priority. When the system needs to process the highest-priority (e.g., most urgent) service request, it can quickly pop the root element (which has the highest priority).</li>
<li>Example: If the system is managing service requests like water leaks (high priority), broken streetlights (medium priority), and potholes (low priority), the Min-Heap allows the system to immediately access the most urgent request. If RequestID = 1 (Water leak) is the most urgent, it is guaranteed to be processed first.
</p></li>



