# Nihongo Memory Coach - PDF content display fixed

Bản này bám theo file index.html gốc người dùng đính kèm, giữ nguyên các tính năng hiện có và sửa phần hiển thị "Nội dung gốc đã trích từ PDF".

Các thay đổi chính:
- Chuẩn hóa ký tự CJK compatibility trong dữ liệu trích từ PDF, ví dụ ⽣ -> 生, ⽬ -> 目, ⾆ -> 舌.
- Sửa các mục bị mất Kanji ở tiêu đề do PDF tách furigana / chữ chính thành nhiều dòng.
- Sửa một số cách đọc bị thiếu âm, ví dụ うけもつ, とりあげる, くりかえす, まわり.
- Làm lại bộ lọc hiển thị nội dung PDF: bỏ dòng furigana rơi rạc, ghép ví dụ bị xuống dòng, chia lại 意味 / ポイント / 例文 / 使い分け / 関連語彙.
- Với Kanji, ví dụ/từ ghép được ghép lại để hiện Kanji chính thay vì chỉ hiện phiên âm.
- Giữ raw text gốc trong phần gập để đối chiếu khi cần.

File audit:
- pdf_content_audit.csv: kiểm tra title so với trang PDF tương ứng.
- pdf_content_title_audit.csv: các title/reading được sửa thủ công từ dữ liệu PDF bị tách dòng.
