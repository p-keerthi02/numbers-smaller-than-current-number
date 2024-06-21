class Solution:
    def smallerNumbersThanCurrent(self, nums: List[int]) -> List[int]:
        x = [0]*len(nums)
        for i in range (len(nums)):
            y=0
            for j in range(len(nums)):
                if nums[j] < nums[i]:
                    y += 1
            x[i] = y
        return x
