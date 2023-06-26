# Module-6-Assignment
# Question 1

import sys

from datetime import datetime

for line in sys.stdin:
    data = line.strip().split("\t")
if len(data) == 6:
    date, time, store, item, cost, payment = data
    time_string = datetime.now().strftime("%H:%M:%S")  # Get the current time
    print("{0}\t{1}\t{2}\t{3}\t{4}\t{5}".format(date, time_string, store, item, cost, payment))
