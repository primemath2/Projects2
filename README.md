# Projects2
Regarding the academic projects.
import math

def standard_deviation(data):
    if len(data) == 0:
        raise ValueError("The data list is empty.")
    
    mean = sum(data) / len(data)
    variance = sum((x - mean) ** 2 for x in data) / len(data)
    return math.sqrt(variance)
