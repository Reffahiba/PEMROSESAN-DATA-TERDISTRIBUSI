import pandas as pd

# Nomor 1
df = pd.read_csv('https://raw.githubusercontent.com/Reffahiba/PEMROSESAN-DATA-TERDISTRIBUSI/main/NVIDIA%20(1999%20-11.07.2023).csv')
df

df = df.drop('Date', axis=1)

means = {}

for column in df.columns:
  values = df[column].tolist()
  total = sum(values)

  mean = total / len(values)
  means[column] =  mean

for column, mean in means.items():
  print(f"{column} : {mean}")

medians = {}

for column in df.columns:
  values = df[column].tolist()
  values.sort()

  n = len(values)
  if n % 2 == 0:
    median = (values[n//2 - 1] + values[n//2]) / 2
  else:
    median = values[n//2]

  medians[column] =  median

for column, median in medians.items():
  print(f"{column} : {median}")

sums = {}

for column in df.columns:
  values = df[column].tolist()
  total = sum(values)

  sums[column] =  total

for column, total in sums.items():
  print(f"{column} : {total}")
