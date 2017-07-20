# traversethroughbinarytree-Java

java class which traverse through a binary tree 
This java class BinaryTree will go through every node of a tree. 
There are lot of other solution for it.
.......

..............


...............


for example ..

public List<Integer> inorderTraversal(TreeNode root) {
    Stack<TreeNode> stack = new Stack<TreeNode>();
    List<Integer> result = new ArrayList<Integer>();
 
    TreeNode p = root;
    while(p!=null){
        stack.push(p);
        p = p.left;
    }
 
    while(!stack.isEmpty()){
        TreeNode t = stack.pop();
        result.add(t.val);
 
        if(t.right!=null){
 
            t= t.right;
            while(t!=null){
                stack.push(t);
                t=t.left;
            }
        }
    }public class Solution {
    List<Integer> result = new ArrayList<Integer>();
 
    public List<Integer> inorderTraversal(TreeNode root) {
        if(root !=null){
            helper(root);
        }
 
        return result;
    }
 
    public void helper(TreeNode p){
        if(p.left!=null)
            helper(p.left);
 
        result.add(p.val);
 
        if(p.right!=null)
            helper(p.right);
    }
}



and lot of other way.... :)


happy coding ...

Samya Ghosh 
Frankfurt , Germany 
 
    return result;
}


or.................................................................



