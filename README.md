# AKA-Lab---Git-Safety-Foundation-Before-Vibe-Coding
*Repository này tạo ra là để thực hành, chuẩn bị cho quá  trình Vibe Coding*

## Lệnh git đã sử dụng:
- **git init** ---           (Khởi tạo kho lưu trữ mới để bật tính năng quản lý phiên bản.)
- **git add** ---            (Gom nhóm các thay đổi có liên quan lại với nhau tại khu vực chuẩn bị, để "ghi nhận" chúng vào lịch sử.)
- **git commit** ---         (Lưu hoặc "lưu lại" các thay đổi trong khu vực dàn dựng vào lịch sử dự án.)
- **git status** ---         (Xem trạng thái hiện tại của thư mục làm việc và khu vực lưu trữ tạm thời.)
- **git checkout** ---       (Thay đổi thư mục làm việc của bạn sang một phiên bản khác từ lịch sử kho lưu trữ.)
- **git log** ---            (Hiển thị lịch sử chi tiết của dự án.)
- **git diff** ---           (Sự khác biệt giữa thư mục làm việc và khu vực dàn dựng.)
- **git revert** ---         (Đảo ngược một commit bị lỗi)
- **git branch** ---         (xem hoặc tạo nhánh)
- **git clone** ---          (tải repository từ GitHub về máy)

## Mục tiêu project:
*Các kỹ năng đã thực hành:*
- Tạo và quản lý GitHub repository
- Sử dụng các lệnh Git cơ bản
- Làm việc với branch
- Tạo pull request
- Xử lý conflict cơ bản
- Rollback/revert khi code bị lỗi
- Hiểu GitHub Flow

## Github flow:
*Github flow gồm các bước:*
- Bước 1: Tạo nhánh mới (Create a branch)
- Bước 2: Thêm commit (Make commits)
- Bước 3: Mở một Pull Request - PR (Open a Pull Request)
- Bước 4: Thảo luận và Đánh giá code (Discuss and Review code)
- Bước 5: Chạy thử nghiệm / Kiểm thử (Deploy for testing)
- Bước 6: Hợp nhất nhánh (Merge và Delete branch)

# 🚀 BÁO CÁO HOÀN THÀNH PROJECT: THỰC HÀNH GIT & GITHUB

Repository này lưu trữ tiến độ, minh chứng hoàn thành các tiêu chuẩn đầu ra của học phần Git/GitHub, đồng thời là móng vững chắc chuẩn bị cho hành trình Vibe Coding sắp tới.

---

## 📌 Khung Kiểm Tra Điều Kiện Hoàn Thành (Checklist)

| STT | Điều Kiện Hoàn Thành | Trạng Thái | Minh Chứng / Vị Trí Kiểm Tra |
| :---: | :--- | :---: | :--- |
| 1 | Hoàn thành các module học tập được giao | ✅ Hoàn thành | Đã học xong lý thuyết |
| 2 | Tạo GitHub repository cá nhân | ✅ Hoàn thành | Chính là Repository này |
| 3 | Có tối thiểu **10 commit** có ý nghĩa | ✅ Hoàn thành | Kiểm tra tại mục **Commits** của Repo |
| 4 | Có tối thiểu **3 branch** thực hành | ✅ Hoàn thành | Nhánh: `main`, `feature-subtract`, `feature-multiply` |
| 5 | Có tối thiểu **2 pull request** | ✅ Hoàn thành | Kiểm tra tại mục **Pull Requests (Closed)** |
| 6 | Có ít nhất **1 tình huống Conflict** | ✅ Hoàn thành | Đã xảy ra và xử lý trực tiếp trên file `main.py` |
| 7 | Có ít nhất **1 tình huống Rollback/Revert** | ✅ Hoàn thành | Đã thực hành lệnh `git revert HEAD` ở commit cuối |
| 8 | Nộp ảnh chụp minh chứng Microsoft Learn | ✅ Hoàn thành | (Học viên đính kèm ảnh bên dưới) |
| 9 | Mentor xác nhận đạt yêu cầu | ⏳ Chờ duyệt | Chờ đánh giá từ Mentor |

---

## 📂 Chi Tiết Các Tình Huống Đã Thực Hành

### 1. Thực Hành Giải Quyết Conflict (Xung đột)
* **Tình huống:** Xảy ra khi thực hiện lệnh `git merge feature-subtract` vào `main`, do file `main.py` ở Local và Remote bị sửa đổi cùng một vị trí một cách độc lập.
* **Cách giải quyết:** Mở file bị xung đột, xóa các ký tự đánh dấu `<<<<<<<`, `=======`, `>>>>>>>`, giữ lại cả 2 nội dung dòng in của Python, sau đó dùng `git add` và `git commit` để hoàn tất.

### 2. Thực Hành Rollback / Revert
* **Tình huống:** Giả lập commit nhầm thư mục rác `__pycache__`.
* **Cách giải quyết:** Sử dụng lệnh `git revert HEAD --no-edit` để Git tự động tạo ra một commit mới đảo ngược lại toàn bộ thay đổi lỗi trước đó mà không làm mất lịch sử dự án.

---

## 🛡️ 10. Nguyên Tắc Bảo Mật Khi Dùng GitHub

Trong quá trình thực hiện dự án này và các dự án tương lai, em luôn tuân thủ nghiêm ngặt các nguyên tắc bảo mật cốt lõi:
* ❌ **Không push mật khẩu** lên GitHub dưới mọi hình thức.
* ❌ **Không push API key hoặc token** cá nhân nhằm tránh bị lộ lọt thông tin hoặc bị bot quét mã khai thác.
* ❌ **Không đưa file `.env`** chứa thông tin cấu hình nhạy cảm lên môi trường public.
* 💡 **Sử dụng file `.gitignore`** ngay từ đầu dự án để tự động loại bỏ các file không cần thiết, file đệm, thư mục rác (như `__pycache__/`, `.env`, `.DS_Store`).
* 🔍 **Kiểm tra kỹ các thay đổi** (sử dụng lệnh `git status` và `git diff`) trước khi tiến hành tạo commit.

---

## 🤖 11. Tôi Sẽ Dùng Git Như Thế Nào Khi Vibe Code Với AI?

Khi bước vào khóa học **Vibe Code**, AI sẽ là trợ lý sinh code rất nhanh nhưng cũng tiềm ẩn rủi ro làm hỏng dự án. Vì vậy, quy trình làm việc an toàn của em sẽ là:

1.  **Không bao giờ sửa đổi trực tiếp trên nhánh `main`**: Giữ nhánh `main` luôn là nơi chứa code sạch và chạy ổn định nhất.
2.  **Quản lý nhánh nghiêm ngặt**: Tạo `branch` độc lập riêng biệt cho từng tính năng hoặc từng thử nghiệm nhỏ trước khi nhờ AI hỗ trợ.
3.  **Kiểm tra và kiểm thử**: Sau khi AI sinh code, em sẽ tiến hành đọc hiểu, rà soát lại lỗi, chạy thử nghiệm tại local, thực hiện `commit` từng bước nhỏ rõ ràng.
4.  **Hợp nhất qua Pull Request**: Chỉ đưa code của AI vào dự án chính thông qua luồng **Pull Request** và kiểm tra xung đột kỹ càng trước khi `merge`.
5.  **Cứu hộ thần tốc**: Nếu AI sinh code lỗi hoặc phá vỡ cấu trúc project, em sẽ dùng sức mạnh của Git để tra cứu lại lịch sử thay đổi (`git log`) và `revert` / `rollback` dự án về trạng thái ổn định gần nhất một cách dễ dàng.

---

## 🏁 12. Kết Luận

Qua project thực hành thực tế này, em đã nắm vững và thao tác thành thạo các kỹ năng Git/GitHub cơ bản, chuẩn bị một tâm thế và nền tảng kỹ thuật vững chắc cho khóa học **Vibe Code**. 

> 📝 **Bài học lớn nhất:** Em hiểu sâu sắc rằng Git không chỉ đơn thuần là công cụ lưu trữ code, mà nó là một "tấm khiên bảo hộ" giúp quản lý mọi sự thay đổi, bảo vệ toàn vẹn mã nguồn, thúc đẩy tinh thần làm việc nhóm chuyên nghiệp và cung cấp cơ chế cứu hộ dự án an toàn mỗi khi có lỗi xảy ra.


