# Mã mời Nado (qp0fptC) 08/2026｜Cách nạp USDC vào Nado? Hướng dẫn đầy đủ: Từ Sàn giao dịch sang Ink L2

Quy trình nạp USDC vào Nado khác với các sàn giao dịch tập trung (CEX). Bạn cần chuẩn bị Web3 Wallet, chuyển tài sản sang mạng Ink L2 và kết nối với Nado. Các lỗi thường gặp bao gồm: chọn sai mạng, quên chuẩn bị ETH cho Gas và chưa chuyển USDC sang Ink.

## Tóm tắt
"Làm sao để nạp USDC vào Nado?"

Khác với CEX, Nado không sử dụng đăng ký tài khoản mà kết nối trực tiếp qua Web3 Wallet.

Quy trình tổng thể:
Mua USDC trên Sàn
↓
Chuyển vào Web3 Wallet
↓
Bridge sang Ink L2
↓
Kết nối Nado
↓
Hoàn tất Deposit (Nạp tiền)

Nado được xây dựng trên hệ sinh thái Ink L2, định vị là Onchain Prime Brokerage (Môi giới chính trên chuỗi), kết hợp ví Web3, giao dịch on-chain và trải nghiệm chuyên nghiệp. Quy trình bắt đầu yêu cầu người dùng chuẩn bị ví, chuyển tiền sang Ink rồi mới nạp vào Nado.

Nếu chưa có tài khoản Nado, bạn có thể sử dụng:
- **📌 Link đăng ký chính thức:** [https://app.nado.xyz?join=qp0fptC](https://app.nado.xyz?join=qp0fptC)
- **📌 Mã mời:** `qp0fptC`

---

## 🌐 1. Tại sao Nado cần mạng Ink L2?
Người mới thường áp dụng tư duy sàn tập trung: Địa chỉ nạp → Chuyển tiền → Giao dịch.
Tuy nhiên, Nado sử dụng mô hình Web3: **Web3 Wallet → Mạng Ink L2 → Nền tảng Nado.**

Ink là mạng Layer 2 trong hệ sinh thái Kraken. Nado dựa vào Ink L2 để cung cấp môi trường giao dịch. Do đó, tài sản phải nằm đúng mạng. Nếu USDC đang ở Ethereum, Arbitrum hoặc tài khoản sàn, bạn cần thực hiện Bridge (chuyển cầu).

---

## 👛 2. Chuẩn bị trước khi dùng Nado
Cần chuẩn bị:

### 1. Web3 Wallet
Nado không dùng Email, Mật khẩu hay Số điện thoại. Kết nối qua ví:
- OKX Wallet
- MetaMask
- Rabby Wallet
- Các ví tương thích EVM khác.

### 2. USDC
Hiện tại Nado chủ yếu dùng **USDC** để giao dịch.
Nếu USDC đang ở Binance, Bybit, OKX, Bitget, hãy rút về Web3 Wallet của bạn.

### 3. ETH cho Gas
Đây là điểm hay bị quên nhất.
Dù ví có USDC, nếu không có đủ **ETH** để trả phí Gas mạng Ink, bạn không thể giao dịch.
Tài liệu chính thức của Ink cũng nhấn mạnh cần có ETH khi dùng công cụ Bridge.

---

## 💳 3. Rút USDC từ Sàn về Wallet
Giả sử USDC đang ở Binance, Bybit hoặc OKX.

**Quy trình cơ bản:**
Tài khoản Sàn → Rút tiền → Chọn USDC → Nhập địa chỉ Wallet → **Xác nhận Mạng (Network)** → Hoàn tất.

⚠️ **Bước quan trọng nhất:** Xác nhận Mạng.
Đừng chỉ nhìn "USDC", hãy chú ý "Network".
USDC trên các chain khác nhau không tương tác trực tiếp được.
- **Khuyến nghị:** Rút về chain tương thích EVM (như Arbitrum, Optimism hoặc Ethereum) để dễ dàng Bridge sang Ink sau này.

---

## 🔗 4. Cách chuyển USDC sang Ink (Bridge)
Nếu USDC đã ở Wallet nhưng chưa ở mạng Ink, bạn cần thực hiện Bridge.

**Quy trình cơ bản:**
Kết nối Wallet → Chọn Bridge → Chọn mạng nguồn → Chọn **Ink** → Xác nhận giao dịch → Chờ xử lý.

Ink cung cấp nhiều công cụ Bridge. Hãy đảm bảo:
- Mạng đích là **Ink**.
- Ví có sẵn một ít **ETH** để trả phí Gas cho việc chuyển cầu.

---

## 📝 5. Kết nối Nado và Nạp tiền lần đầu
Sau khi chuẩn bị xong Ink:

**Bước 1: Truy cập Nado**
- **Link chính thức:** [https://app.nado.xyz?join=qp0fptC](https://app.nado.xyz?join=qp0fptC)
- **Mã mời:** `qp0fptC`

**Bước 2: Kết nối Ví**
Nhấp `Connect Wallet`, chọn ví Web3 của bạn, ký (sign) xác nhận để đăng nhập.

**Bước 3: Xác minh tài sản**
Trong Nado, kiểm tra:
- Ví đã kết nối chưa.
- USDC đã ở trên mạng **Ink** chưa.
- Có đủ **ETH** cho Gas không.

**Bước 4: Hoàn tất Deposit**
Chọn `Deposit`, nhập số lượng USDC, xác nhận giao dịch. Bạn có thể bắt đầu giao dịch.

---

## ⚠️ 6. Các lỗi thường gặp khi nạp Nado

### Lỗi 1: USDC đã về ví nhưng Nado không thấy
**Nguyên nhân:** USDC không ở mạng Ink (ví dụ đang ở Ethereum).
**Cách xử lý:** Kiểm tra mạng và thực hiện Bridge sang Ink.

### Lỗi 2: Giao dịch thất bại liên tục
**Nguyên nhân:**
- Hết ETH Gas.
- Lỗi mạng.
- Chưa xác nhận ký (signature) trên ví.
- Số dư không đủ.

### Lỗi 3: Gửi nhầm địa chỉ?
- **Vào ví tự quản lý:** Thường có thể xử lý được (Bridge ngược lại).
- **Vào địa chỉ nền tảng lạ:** Cần liên hệ hỗ trợ, tỷ lệ thu hồi thấp.
**Lời khuyên:** Luôn thử nghiệm với số tiền nhỏ trước.

---

## 💡 7. Gợi ý cho người dùng lần đầu
Nếu mới làm quen nền tảng on-chain, đừng nạp số tiền lớn ngay.
Quy trình an toàn:
1. Chuẩn bị Ví.
2. Chuyển ít USDC (ví dụ 10-50 USDC).
3. Hoàn tất Bridge sang Ink.
4. Thử nghiệm Deposit.
5. Xác nhận mọi thứ ổn định rồi mới nạp thêm.

Nado khác Binance/Bybit ở chỗ bạn tự kiểm soát tài sản. Hiểu về ví, Gas và Bridge là rất quan trọng.

---

## 📈 8. Sau khi nạp tiền có thể làm gì?
Sau khi USDC vào tài khoản, bạn có thể khám phá hệ sinh thái Nado:
- **Giao dịch Spot (Giao ngay)**
- **Hợp đồng Perpetual (Vĩnh cửu)**
- **Unified Margin (Ký quỹ thống nhất)**
- **Giao dịch On-chain**

Nado không chỉ là DEX đơn thuần, mà hướng tới trải nghiệm giao dịch chuyên nghiệp trên chuỗi.

---

## ❓ Câu hỏi thường gặp (FAQ)

**Q: Nado hỗ trợ nạp tài sản gì?**
A: Hiện tại chủ yếu là USDC. Vui lòng theo dõi thông báo chính thức của Nado để cập nhật.

**Q: Có cần tài khoản sàn giao dịch không?**
A: Không, chỉ cần Web3 Wallet.

**Q: Tại sao phải chuyển USDC sang Ink?**
A: Vì Nado được xây dựng trên hệ sinh thái Ink L2, yêu cầu tài sản phải nằm trên mạng này.

**Q: Nạp tiền Nado có cần Gas không?**
A: Có, giao dịch trên mạng Ink cần ETH để trả phí Gas.

**Q: Mã mời Nado là gì?**
A: `qp0fptC`
Link: [https://app.nado.xyz?join=qp0fptC](https://app.nado.xyz?join=qp0fptC)

**Q: Lần đầu nạp nên gửi bao nhiêu?**
A: Nên dùng số tiền nhỏ để kiểm tra toàn bộ quy trình (Ví -> Bridge -> Deposit) trước khi gửi thêm.

---

## ✅ Tóm tắt
Quy trình nạp tiền vào Nado khác biệt hoàn toàn so với Binance hay Bybit vì nó yêu cầu hiểu biết về Web3 Wallet và Ink L2.

**Quy trình rút gọn:**
**Mua USDC → Rút về Wallet → Bridge sang Ink → Kết nối Nado → Deposit → Giao dịch**

Điểm mấu chốt:
- Đúng mạng.
- Đủ Gas.
- Đúng địa chỉ.
- Thử nghiệm nhỏ trước.

Muốn trải nghiệm Nado?
- **📌 Link chính thức:** [https://app.nado.xyz?join=qp0fptC](https://app.nado.xyz?join=qp0fptC)
- **📌 Mã mời:** `qp0fptC`

Hoàn tất kết nối ví và nạp USDC, bạn đã sẵn sàng khám phá giao dịch on-chain cùng Nado.

---
*Tuyên bố miễn trừ trách nhiệm: Bài viết chỉ mang tính chất tham khảo quy trình. Giao dịch on-chain và cầu nối (Bridge) tồn tại rủi ro hợp đồng thông minh. Vui lòng thận trọng và tự chịu trách nhiệm bảo mật tài sản.*
