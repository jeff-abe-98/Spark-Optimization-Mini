# Spark-Optimization-Mini


This project was meant to work on optimiziation of pyspark processes, but I was unable to get the Adaptive query engine to stop running on my local spark cluster. Any changes I made to the code were not reflected in the execution plan, so troubleshooting was not possible. The only changes I made were switching the order of the join to allow for the smaller frame to be broadcast joined. AQE was already doing that though. I also tried to repartion the data, or order the data before joining, but it had no impact on the execution plan.