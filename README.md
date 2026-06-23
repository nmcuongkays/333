# Nihongo Memory Coach - Final audit build

Bản này giữ nền app có Dễ nhầm, Mazii app-only, dark mode, học/review/quiz/drive mode và thêm các sửa lỗi dữ liệu/hiển thị.

Đã kiểm tra tĩnh:
- JavaScript syntax OK bằng node --check.
- Chỉ còn 1 assignment window.STUDY_DATA.
- Bộ lọc nhanh tìm được bằng Kanji, hiragana và tiếng Việt không dấu.
- Không còn thẻ vocabulary có Kanji mà thiếu cách đọc.
- Không còn tiêu đề lỗi dạng 意味1 / する / やかす / じる.
- Không còn mismatch okurigana đã phát hiện tự động.
- Tab Dễ nhầm, nút Tạo phiên học và hiển thị よみ dưới ví dụ vẫn có trong HTML.

Các file audit:
- display_data_fix_audit.csv: những mục đã sửa.
- remaining_suspects_after_audit.csv: lỗi nghiêm trọng còn lại sau rà soát. File hiện chỉ có header, không còn mục nghiêm trọng.
- raw_split_low_risk_after_audit.csv: các mục PDF gốc tách furigana/kanji nên title không xuất hiện liền trong raw; app đã dùng title/reading sạch để hiển thị.
- final_static_audit_report.txt: kết quả check tĩnh.
