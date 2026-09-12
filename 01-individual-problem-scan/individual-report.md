# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Nguyễn Hoàng Nam
- Mã học viên: 2A202602485
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm cuối ngành CNTT
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):

  - Lập trình tính năng, sửa lỗi (debug) và viết code cho đồ án
  - Đọc tài liệu kỹ thuật, thư viện, API bên thứ ba (chủ yếu bằng tiếng Anh)
  - Viết báo cáo tiến độ đồ án hằng tuần gửi cho Giảng viên hướng dẫn

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được                                                                                                        | Ai chịu ảnh hưởng?                                                              | Dấu hiệu thật (số + bằng chứng)                                                         |
| - | ------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| 1 | Lặp lại                                                                                  | **Viết báo cáo tiến độ đồ án / Standup report hàng tuần cho Giảng viên hướng dẫn**                         | Sinh viên làm đồ án tốn thời gian gõ; GVHD nhận báo cáo muộn            | 60 phút vào cuối tuần để lặp lại các thao tác copy-paste commit, task               |
| 2 | AI có thể làm tốt hơn                                                                 | **Chuyển đổi mô tả yêu cầu (Requirement tiếng Việt) thành Database Schema hoặc API Contract (Swagger/OpenAPI)** | Sinh viên hoặc lập trình viên được giao thiết kế                          | 3-4 tiếng để suy nghĩ thiết kế, hay sót quan hệ bảng và trường dữ liệu          |
| 3 | Pain từ người khác                                                                     | **Thành viên trong nhóm làm đồ án không biết cách setup môi trường chạy dự án**                            | Bạn chưa setup được bị tắc việc; Bạn hỗ trợ bị gián đoạn công việc | Bị hỏi 3-4 lần/tuần đầu, mỗi lần UltraViewer/call mất 30-45 phút                    |
| 4 | Tốn thời gian                                                                            | **Đọc tài liệu API bên thứ ba, thư viện mới**                                                                     | Sinh viên, lập trình viên tích hợp hệ thống                                 | 4-5 tiếng để đọc hiểu docs và đối chiếu mã lỗi                                    |
| 5 | Tốn thời gian                                                                            | **Đọc hiểu tài liệu kỹ thuật tiếng Anh chuyên ngành để nghiên cứu công nghệ mới cho đồ án**            | Sinh viên làm đồ án                                                            | Mất 2-3 tiếng/bài báo hoặc docs tiếng Anh vì phải tra từ điển và ghép ngữ cảnh |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**

- Prompt đã hỏi: "Tôi là sinh viên năm cuối ngành CNTT đang làm đồ án tốt nghiệp và từng đi intern, hãy gợi ý các vấn đề thường gặp theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể làm tốt hơn, pain từ người khác."
- Ý dùng được: Vấn đề viết báo cáo tiến độ tuần từ Git commit, hỗ trợ setup môi trường cho nhóm, đọc docs API và tài liệu tiếng Anh chuyên ngành.
- Ý bỏ vì không phải pain thật: Tự động hóa CI/CD deploy Kubernetes (quá phức tạp cho quy mô đồ án sinh viên), tự động viết toàn bộ code đồ án (viển vông, không thực tế).

**Self-check Phase 1:**

- [X] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [X] Dùng ít nhất 3/4 lăng kính
- [X] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan)                                                                                         | Vì sao chọn (2-3 ý)                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Điều còn chưa chắc                                                                                                                                                                                                                                                      |
| ---- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | **Đọc hiểu tài liệu kỹ thuật tiếng Anh chuyên ngành để nghiên cứu công nghệ mới cho đồ án** | • Sinh viên IT bắt buộc phải đọc docs tiếng Anh để làm đồ án nhưng vốn từ chuyên ngành hạn chế, tốn rất nhiều thời gian tra cứu và dễ hiểu sai kiến trúc.• AI có thế mạnh vượt trội về dịch thuật ngữ cảnh kỹ thuật và tóm tắt luồng kiến trúc sang tiếng Việt trực quan.• Tiết kiệm trực tiếp 2-3 tiếng mỗi khi tiếp cận thư viện/công nghệ mới; tác động trực tiếp đến chất lượng đồ án. | • AI có thể dịch sai các thuật ngữ kỹ thuật mang tính đặc thù hoặc bịa ra cú pháp code mẫu không tương thích (hallucination).• Sinh viên có thể lạm dụng bản tóm tắt mà bỏ qua các cảnh báo bảo mật quan trọng trong tài liệu gốc. |
| 2    | **Thành viên trong nhóm làm đồ án không biết cách setup môi trường chạy dự án**                 | • Pain cực kỳ nhức nhối trong tuần đầu làm việc nhóm, gây gián đoạn công việc của cả người hỏi lẫn người hỗ trợ.• Workflow gỡ lỗi môi trường rất rõ ràng (đọc log lỗi → tìm nguyên nhân thiếu config/version → hướng dẫn sửa).• Đo lường được ngay bằng số lần bị hỏi và thời gian support (giảm từ 45' xuống 5').                                                                                        | • Môi trường mỗi máy tính khác nhau (Windows, MacOS, Linux, phiên bản Node/JDK khác nhau) nên AI có thể chẩn đoán sai lệch.• Người hỏi có thể không biết cách copy đúng đoạn log lỗi đưa cho AI.                                           |
| 3    | **Viết báo cáo tiến độ đồ án / Standup report hàng tuần cho Giảng viên hướng dẫn**              | • Quy trình lặp lại hàng tuần rất chuẩn tắc và cố định (mỗi tối Chủ Nhật).• Bottleneck rõ: bước đọc lại toàn bộ commit Git và task đã làm để gõ thành văn bản mất 40-50 phút.• Dễ dàng kiểm chứng và so sánh giữa làm tay vs dùng AI hỗ trợ.                                                                                                                                                                              | • Giảng viên có thể nhận ra văn phong do AI viết nếu không được người viết chỉnh sửa và biên tập lại.• Nếu tuần đó sinh viên commit ít hoặc message cẩu thả thì AI khó tổng hợp đầy đủ bức tranh tiến độ.                        |

---

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Đọc hiểu tài liệu kỹ thuật tiếng Anh chuyên ngành để nghiên cứu công nghệ mới cho đồ án

```text
Problem 1 câu: Sinh viên IT mất 3-4 tiếng vật lộn đọc tài liệu kỹ thuật tiếng Anh dài (Docs của thư viện mới, RFC, API Docs) do rào cản ngôn ngữ và vốn từ chuyên ngành hạn chế, dẫn đến hiểu sai kiến trúc hệ thống và áp dụng sai code mẫu.

Actor: Sinh viên năm cuối ngành CNTT làm đồ án tốt nghiệp hoặc intern developer khi tiếp cận công nghệ mới.

Thời điểm / bối cảnh: Giai đoạn bắt đầu tích hợp công nghệ/thư viện mới (Docker, Redis, OAuth2, cổng thanh toán, Socket) vào đồ án tốt nghiệp.

Current workflow 3-7 bước:
1. Mở trang Documentation chính thức của thư viện/công nghệ bằng tiếng Anh.
2. Đọc lướt và dùng công cụ dịch từng đoạn văn (nhiều thuật ngữ kỹ thuật bị dịch thô, khó hiểu).
3. Đọc phần Getting Started và Architecture Overview (mất 60-90 phút).
4. Cố gắng chắp vá mã code mẫu vào dự án và chạy thử.
5. Gặp lỗi cú pháp hoặc sai luồng dữ liệu do chưa hiểu bản chất kiến trúc.
6. Quay lại đọc đi đọc lại tài liệu để tìm nguyên nhân (60-90 phút).

Bottleneck: Bước 2 và Bước 3 — Đọc hiểu tài liệu dài và trừu tượng bằng tiếng Anh mất nhiều thời gian nhưng vẫn không nắm được luồng dữ liệu cốt lõi (Core concept).

Impact: Mất 3-4 tiếng mỗi lần tiếp cận thư viện mới; dễ dẫn đến nản chí, trì hoãn hoặc copy-paste code mẫu mà không hiểu bản chất, gây bug tiềm ẩn trong đồ án.

Success metric: Giảm thời gian nắm bắt kiến trúc và cách dùng thư viện từ 3-4 tiếng (180 phút) xuống dưới 35-45 phút; hiểu đúng 100% luồng tích hợp cơ bản.

Non-AI alternative: Tìm video hoặc bài viết blog tiếng Việt (Viblo, TopDev). Nhược điểm: rất ít bài viết tiếng Việt cho các thư viện mới hoặc bài viết đã cũ (outdated) so với phiên bản hiện tại.

AI hypothesis: AI đọc toàn bộ trang tài liệu tiếng Anh, tóm tắt lại kiến trúc bằng tiếng Việt theo sơ đồ luồng dữ liệu (Data Flow) và trích xuất đúng phần code mẫu cần thiết cho bài toán của sinh viên.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1:**

```text
CURRENT STATE — 180 phút (3 tiếng)

[1 Mở docs tiếng Anh: 5'] → [2 Đọc & tra từ điển từng đoạn: 60'] → [3 Đọc Getting Started: 45'] <-- bottleneck → [4 Tự ghép code mẫu: 30'] → [5 Lỗi & đọc lại docs dò lỗi: 40']

FUTURE STATE — 35 phút

[1 Thu thập link docs / nội dung module: 3'] → [2 AI tóm tắt Core Architecture & Luồng dữ liệu bằng tiếng Việt: 5'] → [3 Sinh viên đọc hiểu bản tóm tắt & so sánh với kiến trúc đồ án: 15'] <-- human boundary → [4 AI sinh code boilerplate tích hợp theo context đồ án: 2'] → [5 Sinh viên review code, gắn vào project & test: 10']

Fallback: Nếu AI giải thích khó hiểu hoặc sinh code sai phiên bản thư viện, sinh viên mở lại mục Quickstart trong docs gốc tiếng Anh để đối chiếu.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Hỗ trợ thành viên nhóm setup môi trường dự án & fix lỗi cấu hình

```text
Problem 1 câu: Thành viên trong nhóm đồ án thường xuyên gặp lỗi cấu hình môi trường (sai version runtime, thiếu biến môi trường .env, lỗi kết nối DB) khiến cả người hỏi và người đi hỗ trợ mất 30-45 phút/lần UltraViewer.

Actor: Thành viên gặp lỗi (bị block công việc) và Thành viên hỗ trợ / Leader (bị ngắt quãng công việc).

Thời điểm / bối cảnh: Tuần đầu tiên khởi tạo dự án đồ án hoặc mỗi khi dự án thêm thư viện, dịch vụ mới.

Current workflow 3-7 bước:
1. Thành viên kéo code mới từ Git về máy cá nhân và chạy lệnh khởi động (npm start / mvn spring-boot:run).
2. Terminal báo lỗi đỏ lòm (build failure / exception).
3. Thành viên tự search Google / StackOverflow nhưng không hiểu lỗi đặc thù của dự án (15 phút).
4. Chụp ảnh màn hình gửi vào nhóm Zalo/Discord hỏi xin trợ giúp.
5. Leader hoặc bạn phụ trách phải tạm dừng việc, bật UltraViewer/Google Meet vào máy bạn để kiểm tra từng file config (25-30 phút).
6. Tìm ra nguyên nhân (ví dụ thiếu file .env, sai port DB, sai version Java/Node) và sửa lại.

Bottleneck: Bước 5 — Phải UltraViewer vào máy để mò lỗi thủ công mất 25-30 phút, gián đoạn hoàn toàn mạch làm việc của cả 2 người.

Impact: 3-4 lần/tuần trong giai đoạn setup ban đầu, tiêu tốn tổng cộng khoảng 2-3 tiếng của 2 thành viên; làm chậm tiến độ kick-off dự án chung.

Success metric: Giảm thời gian giải quyết lỗi môi trường từ 40 phút/lần xuống dưới 10 phút; giảm 70% số ca phải UltraViewer trực tiếp.

Non-AI alternative: Viết file README.md hướng dẫn setup chi tiết + file template `.env.example`. Tuy nhiên, người mới thường đọc lướt, bỏ sót bước và README không thể giải thích khi phát sinh log lỗi lạ trên từng hệ điều hành khác nhau.

AI hypothesis: AI được nạp sẵn ngữ cảnh kiến trúc dự án (Tech stack, version chuẩn, các biến môi trường mẫu), khi người dùng dán log lỗi terminal vào, AI sẽ đối chiếu và chỉ chính xác nguyên nhân cùng câu lệnh sửa lỗi.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 45 phút

[1 Kéo code & run: 2'] → [2 Gặp lỗi: 1'] → [3 Tự Google mò mẫm: 15'] → [4 Nhắn tin hỏi nhóm: 2'] → [5 UltraViewer mò lỗi thủ công: 25'] <-- bottleneck

FUTURE STATE — 7 phút

[1 Gặp lỗi terminal: 1'] → [2 Copy log lỗi dán vào Prompt Template dự án: 1'] → [3 AI phân tích log & đối chiếu chuẩn dự án, đưa câu lệnh fix: 1'] → [4 Thành viên tự đọc & chạy lệnh fix: 3'] <-- human boundary → [5 Thành viên xác nhận kết quả: 1']

Fallback: Nếu làm theo lệnh AI đưa ra vẫn không chạy được sau 2 lần thử, mới tạo tin nhắn gửi kèm log và hướng dẫn AI đã thử vào nhóm để Leader can thiệp UltraViewer.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Viết báo cáo tiến độ đồ án / Standup report hàng tuần cho Giảng viên hướng dẫn

```text
Problem 1 câu: Sinh viên mất 45-60 phút mỗi tối Chủ Nhật để lục lại lịch sử Git commit, task Trello và ghi chú rời rạc nhằm viết báo cáo tiến độ tuần gửi Giảng viên hướng dẫn, bước viết tóm tắt mất thời gian và dễ thiếu sót.

Actor: Sinh viên làm đồ án tốt nghiệp (người viết) và Giảng viên hướng dẫn (người đọc).

Thời điểm / bối cảnh: Tối Chủ Nhật hằng tuần, trước buổi họp review tiến độ với GVHD vào đầu tuần.

Current workflow 3-7 bước:
1. Mở GitHub/GitLab xem lại danh sách commit của bản thân và các bạn trong nhóm trong tuần.
2. Mở Trello/Jira xem các thẻ task đã chuyển sang cột "Done" hoặc "In Progress".
3. Mở đoạn chat nhóm trên Zalo xem những khó khăn (blocker) đã gặp phải.
4. Mở Google Docs / Word báo cáo của tuần trước.
5. Tự tay gõ tóm tắt: Đã làm gì, Đang vướng gì, Kế hoạch tuần tới là gì (25-30 phút).
6. Format lại văn bản và gửi email / nộp link lên hệ thống LMS.

Bottleneck: Bước 5 — Tổng hợp từ nhiều nguồn dữ liệu rời rạc (raw logs) thành một văn bản mạch lạc (narrative), thường mất 25-30 phút và dễ bị hiện tượng "ngại viết/bí từ".

Impact: Mất 60 phút/tuần cho mỗi sinh viên. Báo cáo nộp muộn khiến giảng viên không kịp xem trước để chuẩn bị góp ý cho buổi họp đầu tuần.

Success metric: Giảm thời gian viết báo cáo từ 60 phút xuống còn 15 phút; đảm bảo phản ánh chính xác 100% các task quan trọng đã hoàn thành.

Non-AI alternative: Tạo sẵn template báo cáo Word/Notion cố định. Template giúp chuẩn hóa format nhưng không tự tổng hợp commit message hay giải quyết được sự lười gõ narrative của sinh viên.

AI hypothesis: AI nhận đầu vào là danh sách Git log và danh sách task Trello trong tuần, sau đó tự động phân loại thành 3 mục chuẩn: Đã hoàn thành, Vướng mắc (Blocker), Kế hoạch tiếp theo. Sinh viên chỉ cần review và tinh chỉnh trong 5-10 phút.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 60 phút

[1 Soi Git commit: 10'] → [2 Soi task Trello: 10'] → [3 Đọc lại chat blocker: 5'] → [4 Mở Docs: 2'] → [5 Gõ tổng hợp narrative: 28'] <-- bottleneck → [6 Format & gửi: 5']

FUTURE STATE — 14 phút

[1 Export nhanh Git log & danh sách task: 2'] → [2 AI tự động phân loại & soạn thảo bản nháp báo cáo: 2'] → [3 Sinh viên đọc duyệt, bổ sung chi tiết quan trọng & chỉnh sửa: 8'] <-- human boundary → [4 Xuất file PDF / gửi email: 2']

Fallback: Nếu AI tóm tắt sai hoặc bịa thêm task chưa làm, sinh viên dùng template có sẵn và tự điền lại các đầu việc quan trọng.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1: Đọc hiểu tài liệu kỹ thuật tiếng Anh chuyên ngành để nghiên cứu công nghệ mới cho đồ án.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
1. Đọc hiểu tài liệu kỹ thuật tiếng Anh (official docs, RFC, API specs) là rào cản lớn nhất của sinh viên IT khi tiếp cận công nghệ mới làm đồ án tốt nghiệp, dễ dẫn đến nản chí hoặc copy-paste code mẫu mà không hiểu kiến trúc.
2. Workflow rất rõ ràng từ khâu nạp tài liệu tiếng Anh → bóc tách kiến trúc luồng dữ liệu (Data Flow) → sinh code mẫu boilerplate bằng tiếng Việt.
3. Tác động đo đếm được cụ thể: Rút ngắn thời gian đọc hiểu từ 3-4 tiếng (180 phút) xuống còn khoảng 35-45 phút, giúp sinh viên tự tin tích hợp công nghệ mới đúng chuẩn và giảm thiểu lỗi hệ thống.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Tài liệu kỹ thuật tiếng Anh có nhiều phiên bản (v1, v2) và cập nhật liên tục; làm sao đảm bảo AI không tóm tắt dựa trên kiến thức cũ (outdated) hoặc ảo giác (hallucination) ra cú pháp code sai?
2. Liệu việc dựa vào AI tóm tắt có khiến sinh viên lười đọc tài liệu gốc tiếng Anh và bỏ sót các lưu ý quan trọng về bảo mật (security warnings, rate limits)?
```

**AI phản biện Card (nếu có):**

- Điểm yếu AI chỉ ra: AI tóm tắt dễ bỏ sót các cảnh báo quan trọng (caveats, deprecations, security) nằm rải rác trong tài liệu gốc dài hàng chục trang.
- Tôi sửa gì: Thiết kế thêm bước Human Boundary trong workflow: AI bắt buộc phải đính kèm trích dẫn các mục "Important / Security Warning" cùng link neo (anchor link) của tài liệu gốc để sinh viên click vào đối chiếu trực tiếp trước khi code.

### Self-check nộp phần 01

- [X] Có 5+ problems + top 3 Cards đủ field
- [X] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [X] Đã chọn 1 card pitch + câu hỏi challenge
