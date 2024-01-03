# Binary Trees

## Tasks

### Task 0: New node
Write a function that creates a binary tree node.

Prototype: `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`
- `parent` is a pointer to the parent node of the node to create.
- `value` is the value to put in the new node.
- When created, a node does not have any child.
- Your function must return a pointer to the new node, or `NULL` on failure.

### Task 1: Insert left
Write a function that inserts a node as the left-child of another node.

Prototype: `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`
- `parent` is a pointer to the node to insert the left-child in.
- `value` is the value to store in the new node.
- Your function must return a pointer to the created node, or `NULL` on failure or if `parent` is `NULL`.
- If `parent` already has a left-child, the new node must take its place, and the old left-child must be set as the left-child of the new node.

### Task 2: Insert right
Write a function that inserts a node as the right-child of another node.

Prototype: `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`
- `parent` is a pointer to the node to insert the right-child in.
- `value` is the value to store in the new node.
- Your function must return a pointer to the created node, or `NULL` on failure or if `parent` is `NULL`.
- If `parent` already has a right-child, the new node must take its place, and the old right-child must be set as the right-child of the new node.

### Task 3: Delete
Write a function that deletes an entire binary tree.

Prototype: `void binary_tree_delete(binary_tree_t *tree);`
- `tree` is a pointer to the root node of the tree to delete.
- If `tree` is `NULL`, do nothing.

### Task 4: Is leaf
Write a function that checks if a node is a leaf.

Prototype: `int binary_tree_is_leaf(const binary_tree_t *node);`
- `node` is a pointer to the node to check.
- Your function must return `1` if `node` is a leaf, otherwise `0`.
- If `node` is `NULL`, return `0`.

### Task 5: Is root
Write a function that checks if a given node is a root.

Prototype: `int binary_tree_is_root(const binary_tree_t *node);`
- `node` is a pointer to the node to check.
- Your function must return `1` if `node` is a root, otherwise `0`.
- If `node` is `NULL`, return `0`.

### Task 6: Pre-order traversal
Write a function that goes through a binary tree using pre-order traversal.

Prototype: `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`
- `tree` is a pointer to the root node of the tree to traverse.
- `func` is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
- If `tree` or `func` is `NULL`, do nothing.

### Task 7: In-order traversal
Write a function that goes through a binary tree using in-order traversal.

Prototype: `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`
- `tree` is a pointer to the root node of the tree to traverse.
- `func` is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
- If `tree` or `func` is `NULL`, do nothing.

### Task 8: Post-order traversal
Write a function that goes through a binary tree using post-order traversal.

Prototype: `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`
- `tree` is a pointer to the root node of the tree to traverse.
- `func` is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
- If `tree` or `func` is `NULL`, do nothing.

### Task 9: Height
Write a function that measures the height of a binary tree.

Prototype: `size_t binary_tree_height(const binary_tree_t *tree);`
- `tree` is a pointer to the root node of the tree to measure the height.
- If `tree` is `NULL`, your function must return `0`.

### Task 10: Depth
Write a function that measures the depth of a node in a binary tree.

Prototype: `size_t binary_tree_depth(const binary_tree_t *tree);`
- `tree` is a pointer to the node to measure the depth.
