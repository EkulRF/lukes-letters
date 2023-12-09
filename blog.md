---
layout: page
title: All my posts
subtitle: Repository for meandering.
---

<!-- The following JavaScript code fetches and displays the list of posts -->
<script>
    // Specify the directory path
    var directoryPath = "/_posts/";

    // Function to fetch posts from the directory
    function fetchPosts() {
        fetch(directoryPath)
            .then(response => response.text())
            .then(data => {
                // Parse the directory listing
                var parser = new DOMParser();
                var doc = parser.parseFromString(data, "text/html");

                // Extract the list of files
                var files = Array.from(doc.querySelectorAll("a")).map(link => link.getAttribute("href"));

                // Filter out directories and non-post files if needed
                var posts = files.filter(file => !file.endsWith('/') && file.endsWith('.html'));

                // Display the posts on the page
                var postList = document.createElement("ul");
                posts.forEach(post => {
                    var listItem = document.createElement("li");
                    var link = document.createElement("a");
                    link.textContent = post.replace('.html', ''); // Remove file extension if needed
                    link.href = directoryPath + post;
                    listItem.appendChild(link);
                    postList.appendChild(listItem);
                });

                // Append the post list to the document body
                document.body.appendChild(postList);
            })
            .catch(error => console.error("Error fetching posts:", error));
    }

    // Call the fetchPosts function when the page loads
    document.addEventListener("DOMContentLoaded", fetchPosts);
</script>