# Sổ lỗi cần tránh: Trắc địa xây dựng (Chương 3 & 4)

Tài liệu: `study/trac-dia-xay-dung/so-loi.md`  
Cập nhật: Tối thứ Hai 12/10/2026  
Bảng tổng hợp các lỗi sai "chết người" hay gặp nhất trong đề thi và bài giảng của TS. Nguyễn Anh Tài, kèm nguyên nhân bản chất và cách phòng tránh trước khi bước vào phòng thi.

---

| STT | Bài toán / Chủ đề | Lỗi thường gặp | Nguyên nhân bản chất | Cách phòng tránh chuẩn |
|:---:|:---|:---|:---|:---|
| 1 | **Thủy chuẩn từ giữa (Slide 130)** | Lấy $h = b - a$ (ngược dấu chênh cao) | Lấy Trước trừ Sau thay vì Sau trừ Trước | Khắc sâu công thức: $h = a - b = \text{mia sau} - \text{mia trước}$. Điểm trước thấp hơn thì $h < 0$. |
| 2 | **Thủy chuẩn từ giữa (Slide 130)** | Cộng độ cao khi chưa đổi mm sang m | Mia đọc milimét (1000 mm), cao độ tính bằng mét (12.500 m) | Đổi chênh cao ra mét trước: $h\text{ (m)} = h\text{ (mm)} / 1000$. |
| 3 | **Sai số chênh cao (Slide 131)** | Lấy $m_h = m_{đọc}$, quên hệ số $\sqrt{2}$ | Nghĩ rằng đo 1 trạm thì sai số bằng sai số 1 lần đọc | Một trạm đọc 2 mia: $m_h = \sqrt{m_a^2 + m_b^2} = m_{đọc}\sqrt{2}$. Luôn nhân $\sqrt{2}$. |
| 4 | **Bài toán ngược sai số (Slide 131)** | Lấy trực tiếp $5$ mm làm $m_{đọc}$ | Không giải bất đẳng thức truyền sai số | $m_{đọc}\sqrt{2} \le 5 \implies m_{đọc} \le 5/\sqrt{2} \approx 3.536$ mm. |
| 5 | **Đo khoảng cách thị cự (trang 67)** | Quên nhân hệ số 2 khi mất chỉ trên | Lấy $(c_g - c_d) \times 100$ trực tiếp | Khi chỉ có chỉ giữa và chỉ dưới: $D = 200 \times (c_g - c_d)$ hoặc tính $c_t = 2c_g - c_d$ trước. |
| 6 | **Lượng giác công trình (Slide 145)** | Quên dấu âm của góc chúc xuống $V_C$ | Góc ngắm xuống chân $V_C = -20^\circ 30'$ mang dấu âm | Bấm máy: $\tan V_Đ - \tan(-20.5^\circ) = \tan V_Đ + \tan(20.5^\circ)$. Chiều cao công trình luôn $> 0$. |
| 7 | **Lượng giác công trình (Slide 145)** | Bấm $\tan(V_Đ - V_C)$ gộp chung | Nhầm lẫn tính chất toán học lượng giác | $\tan(A - B) \neq \tan A - \tan B$. Bắt buộc phải tính riêng từng giá trị $\tan$ rồi trừ nhau! |
| 8 | **Lượng giác công trình (Slide 145)** | Đổi phút sai: lấy $30' = 0.30^\circ$ | Lẫn lộn giữa hệ thập phân và lục thập phân | $30' = 30/60 = 0.5^\circ$. Góc $15^\circ ZZ' = (15 + ZZ/60)^\circ$. |
| 9 | **Lượng giác công trình (Slide 146)** | Bỏ thi vì đề không cho chiều cao máy $i$ | Không nhận ra tính chất triệt tiêu | Chiều cao công trình $h_{CĐ} = H_Đ - H_C = D(\tan V_Đ - \tan V_C)$, đại lượng $i$ tự triệt tiêu. |
| 10 | **Bình sai độ cao (Slide 198)** | Thay cự ly mét vào căn tính $f_{hcp}$ | Quên quy ước đơn vị của công thức $50\sqrt{L}$ | Chiều dài $L$ bắt buộc phải đổi sang **kilômét (km)**: $520$ m $= 0.520$ km $\implies 50\sqrt{0.520} \approx \pm 36$ mm. |
| 11 | **Bình sai độ cao (Slide 198)** | Đảo dấu sai số khép $f_h$ | Lấy $(H_{đầu} - H_{cuối})$ thay vì $(H_{cuối} - H_{đầu})$ | Luôn nhớ: $f_h = \sum h_{đo} - (H_{cuối} - H_{đầu})$. Số hiệu chỉnh $v_i = -f_h \cdot \dots$ (ngược dấu $f_h$). |
| 12 | **Bình sai theo trạm (Slide 199)** | Làm tròn cứng nhắc làm lệch tổng $\sum v$ | Làm tròn $-0.01576$ thành $-0.016$ làm tổng thành $-0.068 \neq -0.067$ | Kiểm tra bắt buộc: $\sum v_i = -f_h$. Nếu bị lệch 1 mm, điều chỉnh 1 mm ở đoạn dài nhất hoặc trạm nhiều nhất để khớp tổng. |
| 13 | **Mốc công trình A (Slide 200/201)** | Lấy trực tiếp $h_{AN1}$ cho đoạn $N_1 \to A$ | Chiều đo ngược chiều tiến của tuyến | Tuyến $N_1 \to A \to N_2$ có đoạn đầu là từ $N_1$ đến $A$, phải đổi dấu: $h_{N1A} = -h_{AN1} = -(-0.225) = +0.225$ m. |
| 14 | **Truyền góc định hướng (trang 96)** | Nhầm công thức giữa góc trái và góc phải | Không chú ý góc đo nằm bên nào theo chiều tiến | Góc bên **Trái** (chuẩn giáo trình trang 96–98): $\alpha_{sau} = \alpha_{trước} + \beta_{trái} - 180^\circ$. Góc bên **Phải**: $\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}$. |
| 15 | **Bài toán nghịch tọa độ (trang 94)** | Nhầm góc định hướng giữa các góc phần tư | Máy tính chỉ trả về $\arctan$ trong khoảng $(-90^\circ, +90^\circ)$ | Xét dấu $\Delta X, \Delta Y$: (+,+) giữ nguyên; (-,+) lấy $180^\circ - r$; (-,-) lấy $180^\circ + r$; (+,-) lấy $360^\circ - r$. |
| 16 | **Kiểm nghiệm máy thủy chuẩn (trang 68)** | Lắc mia lấy số đọc lớn nhất | Nhầm tính chất hình học tam giác vuông | Mia nghiêng tạo cạnh huyền (dài hơn), mia thẳng đứng là cạnh góc vuông (ngắn nhất) $\implies$ Lắc mia phải lấy **SỐ ĐỌC NHỎ NHẤT**. |
