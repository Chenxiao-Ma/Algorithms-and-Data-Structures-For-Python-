回溯算法模板：

    result = []
    def backtrack(路径, 选择列表):
        if 满足结束条件:
            result.add(路径)
            return
        
        for 选择 in 选择列表：
            做选择
            backtrack(路径, 选择列表)
            撤销选择
            
        <labuladong的算法小抄-page43>

Tips with BackTracking:
1.解决一个回溯问题，实际上就是一个决策树的遍历过程
2.回溯法的本质，也是在穷举

The Difference between BackTracking and DFS:
1."回溯法 = 深度优先搜索 + 剪枝" 并不准确，
