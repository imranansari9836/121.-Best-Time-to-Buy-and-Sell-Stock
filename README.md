class Solution {
    public int maxProfit(int[] prices) {
        int maxProfit=0;
        int minSofar=prices[0];//7
        for(int i=0;i<prices.length;i++)
        {
            minSofar=Math.min(minSofar,prices[i]);//7,7=7
            int profit=prices[i]-minSofar;//7-7=0
            maxProfit=Math.max(maxProfit,profit);//0,0=0//5
        }
        return maxProfit;//5
    }
}
