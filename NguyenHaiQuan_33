import pandas as pd

data = {
    "Ho_ten": [
        "An", "Binh", "Chi", "Dung", "Ha",
        "Hung", "Lan", "Minh", "Nam", "Vy"
    ],
    "Chuyen_can": [8, 9, 7, 6, 10, 8, 7, 9, 5, 8],
    "Giua_ky":    [7, 8, 6, 7, 9, 8, 6, 7, 5, 9],
    "Cuoi_ky":    [9, 8, 7, 5, 9, 7, 8, 9, 4, 8]
}

df = pd.DataFrame(data)

print(df)
print("So sinh vien:", len(df))
print("So cot:", len(df.columns))
df["Tong_Ket"] = (
    0.2 * df["Chuyen_can"]
    + 0.3 * df["Giua_ky"]
    +0.5 * df["Cuoi_ky"]
)

print(df)
def xep_loai(diem):
  if diem >= 8.5:
    return "Gioi"
  elif diem >= 7.0:
    return "Kha"
  elif diem >= 5.0:
    return "Trung Binh"
  else:
    return "Yeu"

df["Xep_loai"] = df["Tong_Ket"].apply(xep_loai)
print(df.to_string(index=False))

print("\nSo sinh vien:", len(df))
print("So cot:", len(df.columns))
