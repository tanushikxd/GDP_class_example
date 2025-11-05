This project is an example based on class materials, where our goal was to understand how tools such as:

matplotlib.plot
seaborn
sqllite
work in real projects. Based on guidance, I've run several codes, to find out the outcome of information which was really meaningfull to me.

Dataset souce: Provided by JustIt, you can find it in the 'data' folder

After reviewing dataset, i felt very curious about the exact numbers on several points:

1. TOP 10 countries across the world by IMF (international monetary fund), that information personally felt very important for me.

top_countries = df.sort_values("IMF_Estimate", ascending=False).head(10)

![alt text](<visuals/top-10 by IMF.png>)

2. In this section i got curious about the Estimated GDP by regions and as an outcome i've created 2 visual tools - barchart and boxchart to get more clear understanding

top_regions = df.groupby("UN_Region")[["IMF_Estimate","WorldBank_Estimate","UN_Estimate"]].mean()

![alt text](<visuals/top-10 by region in bar.png>)

![alt text](<visuals/top-10 by region.png>)
