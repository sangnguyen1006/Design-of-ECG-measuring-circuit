# Design-of-ECG-measuring-circuit
## Mạch điện tim bao gồm:
    • Các mạch khuếch đại đo lường: khuếch đại tín hiệu 
    • Lọc thông cao: loại bỏ tín hiệu DC
    • Lọc thông thấp: lấy giới hạn băng thông ở các tần số cần quan tâm
    • Lọc triệt dải 50 Hz: loại bỏ nhiễu 50Hz khỏi tín hiệu ECG
    • Mạch tách sóng R: bộ dò QRS
    
## Thiết bị và phần mềm cần dùng trong TN:
    • Máy tim giả : Máy phát tín hiệu điện tim, có nhiệm vụ tạo ra tín hiệu
    điện tim giống như trên người. Trong bài báo cáo này, nhóm chọn đo ở 
    đạo trình I, với biên độ điện tim = 1mV, 80 bpm.
    • Máy tạo sóng: tạo sóng hình sin kiểm tra mạch khuếch đại, mạch lọc (high pass, 
    low pass, band pass, notch pass).
    • Máy Oscilloscope: Sử dụng 2 kênh đo tín hiệu tương tự để so sánh/đối chiếu 
    tín hiệu vào và ra.
    • Phần mềm proteus: thiết kế PCB.
    
## Thực hiện:
    • Sử dụng IC khuếch đại thuật toán LM324N, biến trở ở nhiều giá trị khác nhau 
    để điều chỉnh chính xác giá trị R mong muốn.
    • Test mạch trên máy phát sóng ECG (Biên độ 1mV,F=2Hz )
    • Sử dụng nguồn đôi: ±5V
    • Tín hiệu thu được sau khi qua bộ dò QRS (khuếch đại tần số sóng QRS và 
    loại bỏ qua tần số sóng khác)
    
## Kết quả thực hành:
    • Vẽ PCB và làm mạch đo ECG
    • Hiệu chỉnh mạch (tần số cắt)
    • Test mạch trên máy phát sóng ECG 
    • Tín hiệu ra với biên độ 920mV (khuếch đại ~1000 lần),  
    F=2Hz, thời gian trung bình 2 đỉnh R-R= ~0,5s (~120 nhịp/phút).
