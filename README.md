                                               Explanation of Data structures 
<ol>The structures that I used are Binary search tree and Mini-Heap</ol>
<li></li>Binary Search Tree (BST)<li></li>
•	Role: The BST helps store and manage the Service Request Model objects. It helps to organize the requests by their RequestID, this makes it efficient to search for specific requests based on their ID. The key idea behind the BST is that for each node, all elements in the left subtree are smaller, and all elements in the right subtree are greater. This structure ensures that the searching operation that is finding a request by its ID, happens in O (log n) time complexity, where n is the number of requests in the tree.

<ol></ol>	Efficiency Contribution:</ol>
o	Searching: this helps to quickly find any service using the RequestID by using the Search method. Instead of searching through all the requests sequentially, the BST allows you directly jump to the correct node, drastically improving search time.
o	Example: If a user wants to track a specific service request (for example they want to search for RequestID number 3), the BST will efficiently locate that request, and return its details (Description as well as their Status) without having to search through all requests.
o	In-Order Traversal: The BST can also be traversed in in-order to retrieve all the requests in ascending order of RequestID. This ensures that the requests are displayed in a sorted manner in the UI.
Min-Heap
•	Role: The Min-Heap is used to manage the priority of service requests. It is used to store requests based on their Priority level, where the highest-priority request (lowest priority number) is always at the root. A Min-Heap ensures that when you need to retrieve or process the highest-priority request, it can be done in O (log n) time.
•	Efficiency Contribution:
o	Priority Management: The service requests are inserted into the Min-Heap with their priority. When the system needs to process the highest-priority (e.g., most urgent) service request, it can quickly pop the root element (which has the highest priority).
o	Example: If the system is managing service requests like water leaks (high priority), broken streetlights (medium priority), and potholes (low priority), the Min-Heap allows the system to immediately access the most urgent request. If RequestID = 1 (Water leak) is the most urgent, it is guaranteed to be processed first.

