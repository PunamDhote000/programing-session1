1.class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        return nums + nums

2.class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        return nums * 2

3.class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        ans = []
        ans.extend(nums)  
        ans.extend(nums)  
        return ans

4.class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        ans = nums[:]  
        ans.extend(nums)  
        return ans

 5.class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        return [nums[i] for i in range(len(nums))] + [nums[i] for i in range(len(nums))]

