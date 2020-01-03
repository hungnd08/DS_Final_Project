# DS_Final_Project
## Thành viên
|**STT**|**MSSV**|**Họ và tên**|  
|:---:|:---:|---|  
|1|1612272|Trần Nhật Huy|
|2|1512222|Nguyễn Duy Hưng|  

## Quá trình làm việc nhóm
### I. Họp nhóm và phân công công việc
* **Lần 1**  
Ngày: 24/11/2019  
Địa điểm: Facebook

|**Công việc**|**Ngày thực hiện**|**Người làm**|  
|---|:---:|---|  
|Crawl dữ liệu|26/11/2019|Nguyễn Duy Hưng|  
|Viết báo cáo|30/11/2019|Trần Nhật Huy|

* **Lần 2**  
Ngày: 2/1/2020  
Địa điểm: Facebook  

|**Công việc**|**Ngày thực hiện**|**Người làm**|  
|---|:---:|---|  
|Thống nhất kế hoạch làm|2/1/2020|Trần Nhật Huy, Nguyễn Duy Hưng|  
|Viết kế hoạch và chỉnh sửa|3/1/2020|Trần Nhật Huy, Nguyễn Duy Hưng|  
|Viết báo cáo|6/1/2020|Trần Nhật Huy|  
|Slide|6/1/2020|Nguyễn Duy Hưng|  

### II. Kế hoạch làm
1. Chọn đặc trưng  
Dữ liệu hiện tại của nhóm gồm 11 cột với cột `humidity` là cần dự đoán. Nhóm dự tính sẽ bỏ cột `visibility`, `apparentTemparature` vì nhóm nhận thấy 2 cột này không có ảnh hưởng đến độ ẩm. Cột `time` nhóm sẽ tách ra thành 2 cột là `date (Ngày bao nhiêu trong tháng đó)` và `month` và bỏ đi cột `time` => Dữ liệu train bây giờ sẽ có 9 đặc trưng

2. Các model nhóm sẽ huấn luyện  
Dữ liệu của nhóm sẽ chia làm 3 tập `train`, `validation` và `test` theo tỉ lệ `6:2:2`  
Nhóm sẽ lựa chọn model `Linear Regression`  
Các cột có giá trị thiếu nhóm sẽ lần lượt thử các phương pháp `mean`, `median`, `mode`, `k nearest neighbor` => Thử trên tập `validation` => Chọn phương pháp tốt nhất (1)  
Nhóm sẽ chọn đặc trưng bằng `PCA` với `n` chạy từ `[4:8]` => Thử trên tập `validation` => Chọn phương pháp tốt nhất (2)  
Kết hợp (1) và (2) nhóm sẽ chọn ra phương pháp có độ chính xác trên tập `validation` lớn nhất và tiến hành train lại trên tập `train` và `validation` 






