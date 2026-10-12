# Hướng dẫn cho Antigravity: ôn thi Trắc địa xây dựng (chương 3 và 4)

Đọc hết file này trước khi làm. Làm liên tục, không dừng để hỏi. Các điểm chưa rõ thì ghi vào mục "Cần hỏi thầy" ở báo cáo cuối.

## 1. Bối cảnh

- Người học là sinh viên xây dựng. Ngày mai (thứ ba 13/10/2026) thi giữa kỳ môn Trắc địa xây dựng.
- Phạm vi: chương 3 và chương 4 của giáo trình. Thầy nói phần lớn đề lấy từ 18 ảnh chụp bài giảng.
- Thư mục làm việc: `C:\Workspace\01_Projects\HeThong\study\trac-dia-xay-dung\`. Chỉ tạo và ghi file trong thư mục này.
- Giáo trình: `C:\Workspace\01_Projects\HeThong\Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf` (156 trang). Đọc bằng PyMuPDF (`pip install pymupdf`). Đọc mục lục trước, rồi chỉ đọc chương 3 và 4. Theo ghi chú cũ, chương 3 khoảng trang 37–70 và chương 4 khoảng trang 71–114. Kiểm tra lại theo mục lục.
- Ảnh bài giảng: 18 file `.jpg` nằm trong `C:\Workspace\01_Projects\HeThong\`. Danh sách và số slide ghi trong `nguon.md`.
- Không sửa, không xóa file gốc (PDF và ảnh).
- Nếu skill `civil-eng-essence-study` đã có trong Antigravity, làm theo quy trình của skill. Nếu không, làm theo các quy tắc trong file này.

## 2. Đề thi đã biết

- Câu 2 (2 điểm): đo cao lượng giác, tính chiều cao công trình khi không tới chân mia (slide 145, 146).
- Câu 3 (3 điểm): thủy chuẩn từ giữa M→N. Mục 3.1 và 3.2 mỗi mục 0,5 điểm. Mục 3.3 và 3.4 mỗi mục 1 điểm (slide 130, 131).
- Bình sai tuyến đo cao và bài tập mốc công trình (slide 196 đến 201). Số điểm chưa rõ.
- Câu 1: chưa có ảnh, chưa biết nội dung. Ghi là "chưa rõ", không tự bịa.
- ZZ trong đề là số riêng của người học. Viết công thức theo ZZ, và có bảng thay số cho vài giá trị ZZ để luyện.

## 3. Việc cần làm, theo thứ tự ưu tiên

1. Đọc lại 18 ảnh. Chép đề và lời giải của từng slide vào `de-va-loi-giai-anh.md`. Dùng Python kiểm tra mọi phép tính, không tính nhẩm. Nếu lời giải trên slide sai thì ghi rõ, không sửa im lặng.
2. Đối chiếu các file khái niệm đang có với giáo trình: thuy-chuan-hinh-hoc.md, do-cao-luong-giac.md, danh-gia-sai-so-do-cao.md, binh-sai-tuyen-do-cao.md, binh-sai-duong-chuyen-kinh-vi.md, hai-bai-toan-trac-dia.md. Sửa chỗ sai và ghi trang nguồn.
3. Cập nhật `luyen-tap.md`: mỗi dạng bài có ít nhất 3 bài, có lời giải từng bước. Mỗi lời giải phải tự kiểm được: đổi đơn vị, xét dấu, tổng số hiệu chỉnh bằng −f_h, độ cao cuối khớp mốc.
4. Viết `de-thi-du-kien.md`: một đề thử 10 điểm theo cấu trúc ở mục 2, có đáp án theo ZZ.
5. Thêm file cho các mục chương 3 và 4 còn thiếu so với mục lục giáo trình, mỗi mục một file theo mẫu chín mục của skill. Làm sau cùng, theo thời gian còn lại.
6. Cập nhật `to-cong-thuc.md` (tối đa một trang), `so-loi.md`, `ban-do.md`, `nguon.md`, `ke-hoach.md` cho khớp với các file mới.

Các file hiện có đã được sửa một lần ngày 12/10. Đọc trước khi sửa, không làm lại từ đầu.

## 4. Quy tắc chất lượng

- Mọi số liệu lấy từ giáo trình hoặc ảnh, kèm nguồn: tên file và trang, hoặc tên file ảnh và số slide. Kiến thức ngoài tài liệu ghi nhãn [ngoài tài liệu]. Thiếu số liệu thì ghi "cần tra", không bịa.
- Số đọc mia tính bằng mm. Độ cao và chênh cao tính bằng m (chia 1000). Ghi đơn vị cạnh mỗi công thức.
- Công thức đã kiểm tra, dùng làm chuẩn:
  - Thủy chuẩn từ giữa: h_AB = a − b, với a là chỉ giữa mia sau và b là chỉ giữa mia trước. Đổi chiều tuyến thì đổi dấu h.
  - Sai số một trạm từ giữa: m_h = m_đọc × √2. Bài toán ngược: m_đọc ≤ m_h,cp / √2.
  - Đo cao lượng giác: h = D·tanV + i − l. V âm khi ngắm xuống. Chiều cao công trình gián tiếp: h_CĐ = D(tanV_Đ − tanV_C). Khi ngắm sát điểm (l = 0) thì không cần i.
  - Bình sai tuyến phù hợp: f_h = Σh_đo − (H_cuối − H_đầu). f_hcp = ±50√L (mm, L tính bằng km) hoặc ±10√N (mm, N là số trạm). Nếu đề cho f_hcp thì dùng số đề cho.
  - Số hiệu chỉnh: v_i = −f_h·D_i/ΣD hoặc v_i = −f_h·n_i/N. Kiểm tra Σv = −f_h. Chênh cao sau bình sai: h^BS = h_đo + v. Độ cao: H_i = H_{i−1} + h^BS.
  - Truyền góc định hướng: α_sau = α_trước + β_phải − 180°, với β đo bên phải theo chiều tiến. Bản cũ ghi sai dấu, đã sửa.
- Thuật ngữ tiếng Việt, thuật ngữ tiếng Anh trong ngoặc ở lần đầu xuất hiện. Mỗi file khái niệm không quá hai trang in.

## 5. Thời gian

Người học còn khoảng 3 giờ tối nay. Làm xong việc 1, 3 và 4 trước. Việc 2 và 5 làm tiếp theo thứ tự. Sau mỗi file xong, thêm tên file vào cuối `ke-hoach.md`.

## 6. Báo cáo cuối

Liệt kê:
- File đã tạo hoặc sửa.
- Phần đã đối chiếu với giáo trình.
- Phần chưa đối chiếu.
- Mục "Cần hỏi thầy": nội dung Câu 1, số điểm của phần bình sai, và f_hcp của đề nếu đề có cho.
