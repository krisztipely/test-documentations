# User story e-commerce

## User story

As a user, I want to be able to search for products on an e-commerce website, so that I can quickly find and purchase items I am interested in.

## Test cases

**Positive test case - Basic search**

Input: User enters a valid search query (test data: laptop)
Expected outcome: The search results display relevant products matching the query.

**Positive test case - Advanced search**

Input: User uses advanced search filters (test data: price range, brand)
Expected outcome: The search results reflect the specified data accurately.

**Negative test case - Empty search**

Input: User attempts to search without entering any query.
Expected outcome: The system prompts the user to enter a search query.

**Negative test case - Invalid search**

Input: User enters a non-existent product name or random characters.
Expected outcome: The system provides a message indicating that no matching products were found.

**Boundary test case - Maximum search results**

Input: User performs a broad search resulting in the maximum number of displayed products.
Expected outcome: The system correctly displays the maximum number of products allowed per page.

**Performance test case - Response time**

Input: User performs a search, and response time is measured.
Expected outcome: The search results load within an acceptable time frame.

