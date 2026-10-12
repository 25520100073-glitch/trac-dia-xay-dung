# Kiểm nghiệm máy thủy chuẩn (chương 3) [ngoài tài liệu]

Phần này chưa đối chiếu với giáo trình. Trước khi dùng cho bài thi, đối chiếu mục về kiểm nghiệm và chỉnh máy thủy chuẩn.

## 1. Vì sao phải kiểm nghiệm

Đo chênh cao bằng thủy chuẩn dựa vào tia ngắm nằm ngang. Điều kiện chính là trục ngắm CC1 song song với trục bọt thủy dài LL1. Nếu không song song, tia ngắm nghiêng một góc $i$, và chênh cao đo trực tiếp sẽ sai một lượng tỉ lệ với khoảng cách.

## 2. Vì sao đặt máy giữa hai mia thì triệt được sai số i

Khi máy cách đều hai mia, sai số do $i$ ở mia sau và mia trước bằng nhau về độ lớn, cùng chiều. Khi tính $h = a - b$, hai sai số này bù trừ nhau. Vì vậy chênh cao đo từ giữa không phụ thuộc $i$. Đây là lý do thủy chuẩn từ giữa được dùng nhiều nhất.

## 3. Phương pháp hai điểm

1. Chọn hai điểm A và B cách nhau khoảng 40 đến 60 m. [ngoài tài liệu, khoảng cách gợi ý]
2. Đặt máy đúng giữa A và B. Đọc $a_1$ (mia A), $b_1$ (mia B). Tính $h_1 = a_1 - b_1$. Đây là chênh cao đúng.
3. Đặt máy gần A, cách mia A khoảng 2 đến 3 m. Đọc $a_2$ (mia A), $b_2$ (mia B). Tính $h_2 = a_2 - b_2$. Khi máy gần A, sai số ở mia A rất nhỏ, nên sai số $i$ nằm chủ yếu ở mia B.
4. Tính sai số $i$ theo giây:

$$i'' = \frac{(h_1 - h_2)\cdot 206265}{D_{AB}}$$

với $D_{AB}$ là khoảng cách giữa A và B. [ngoài tài liệu]

5. So $i''$ với giới hạn cho phép trong giáo trình hoặc hướng dẫn máy. [cần tra giới hạn]. Nếu vượt, chỉnh vít điều chỉnh để tia ngắm nằm ngang, rồi kiểm lại.

## 4. Tự kiểm tra

1. Vì sao đặt máy giữa hai mia thì chênh cao không phụ thuộc $i$? Đáp: sai số ở hai mia bằng nhau về độ lớn và cùng chiều, nên khi lấy hiệu $a - b$ thì triệt tiêu.
2. Hai điểm cách nhau 50 m. Khi máy đặt giữa: $h_1 = +0{,}120$ m. Khi máy đặt gần A: $h_2 = +0{,}110$ m. Tính $i''$. Đáp: $i'' = (0{,}120 - 0{,}110)\times 206265 / 50 \approx 41$ giây. [ngoài tài liệu, chỉ để luyện công thức]
