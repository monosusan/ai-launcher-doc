- [English](./README.md)
- [简体中文](./README.ZH-CN.md)
- [正體中文](./README.ZH-TW.md)
- [हिन्दी](./README.HI-IN.md)
- [Français](./README.FR.md)
- [한국어](./README.KO.md)
- [Español](./README.ES.md)
- [Polski](./README.PL.md)
- [Nederlands](./README.NL.md)
- [Deutsch](./README.DE.md)
- [日本語](./README.JA.md)
- [Tiếng Việt](./README.VI.md)
- [Türkçe](./README.TR.md)

## Bắt Đầu Nhanh

1. Mua trên Trang Web Chính Thức AI Launcher
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Sau khi thanh toán, truy cập Trung Tâm Đơn Hàng
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Chọn đơn hàng của bạn để kích hoạt.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Liên kết tên người dùng Github của bạn để kích hoạt
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Sau khi kích hoạt thành công, bạn sẽ nhận được lời mời trong thông báo Github. Nhấp để tham gia kho mã nguồn AI Launcher.

## Sao Chép Mã Nguồn Dự Án

1. Truy cập Kho Mã Nguồn AI Launcher (hiển thị 404 nếu bạn không phải là thành viên)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Chọn sao chép Git hoặc tải mã nguồn trực tiếp về máy tính của bạn

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Cài Đặt Dự Án

1. Di chuyển đến thư mục gốc của dự án
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Cài đặt các gói phụ thuộc của dự án

   ```bash
   pnpm install
   ```

## Phát Triển và Gỡ Lỗi

1. Sao chép tệp cấu hình biến môi trường

   ```bash
   cp .env.example .env.development
   ```

2. Khởi chạy máy chủ phát triển

   ```bash
   pnpm dev
   ```

3. Xem Trước Cục Bộ
   
   Mở [http://localhost:3000](http://localhost:3000/) trong trình duyệt để xem dự án

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Tùy Chỉnh

### Thay Đổi Màu Sắc Trang Web

1. Chọn trình gỡ lỗi chủ đề shadcn
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Tạo bảng màu cho dự án của bạn

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Sao chép kiểu chủ đề và dán vào tệp dự án của bạn

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Làm mới trang xem trước dự án để xem chủ đề tùy chỉnh

### Thay Đổi Nội Dung Trang Chủ

1. Mở tệp nội dung trang chủ và sử dụng AI để tạo nội dung mới

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Áp dụng nội dung được tạo bởi AI, thực hiện chỉnh sửa thủ công và xem trước trang chủ mới
3. Tiếp tục tùy chỉnh các tệp JSON khác để nội dung trang web phù hợp với dự án của bạn

### Thay Đổi Văn Bản Đa Ngôn Ngữ

Trong thư mục, cấu hình nội dung trang thông qua các tệp. Tiếng Trung và tiếng Anh được hỗ trợ mặc định. Điều chỉnh văn bản cho dự án của bạn trước khi ra mắt.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

Bạn có thể sử dụng AI để tạo nội dung.

### Thay Đổi Chính Sách Trang Web

Trước khi chính thức ra mắt trang web, hãy cập nhật chính sách trang web theo dịch vụ của bạn.

1. Cập Nhật Chính Sách Bảo Mật
   
   Trong Windsurf, sử dụng prompt để tạo nội dung chính sách bảo mật mới.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Thay thế nội dung tệp để cập nhật chính sách bảo mật.

2. Cập Nhật Điều Khoản Dịch Vụ
   
   Trong Windsurf, sử dụng prompt để tạo nội dung điều khoản dịch vụ mới.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Thay thế nội dung tệp để cập nhật điều khoản dịch vụ.

## Thay Đổi Biến Môi Trường

Sửa đổi các biến môi trường theo nhu cầu thực tế để bật lưu trữ dữ liệu/đăng nhập/phân tích/thanh toán và các tính năng khác

```env
# -----------------------------------------------------------------------------
# Web Information
# -----------------------------------------------------------------------------
NEXT_PUBLIC_WEB_URL = "http://localhost:3000"
NEXT_PUBLIC_PROJECT_NAME = "AI Launcher"

# -----------------------------------------------------------------------------
# Database with Supabase
# -----------------------------------------------------------------------------
# https://supabase.com/docs/guides/getting-started/quickstarts/nextjs
# Set your Supabase URL and Anon Key
SUPABASE_URL = ""
SUPABASE_ANON_KEY = ""
SUPABASE_SERVICE_ROLE_KEY = ""

# -----------------------------------------------------------------------------
# Auth with next-auth
# https://authjs.dev/getting-started/installation?framework=Next.js
# Set your Auth URL and Secret
# Secret can be generated with `openssl rand -base64 32`
# -----------------------------------------------------------------------------
AUTH_SECRET = ""

# Google Auth
# https://authjs.dev/getting-started/providers/google
AUTH_GOOGLE_ID = ""
AUTH_GOOGLE_SECRET = ""
NEXT_PUBLIC_AUTH_GOOGLE_ID = ""
NEXT_PUBLIC_AUTH_GOOGLE_ENABLED = "false"
NEXT_PUBLIC_AUTH_GOOGLE_ONE_TAP_ENABLED = "false"

# Github Auth
# https://authjs.dev/getting-started/providers/github
AUTH_GITHUB_ID = ""
AUTH_GITHUB_SECRET = ""
NEXT_PUBLIC_AUTH_GITHUB_ENABLED = "false"

# -----------------------------------------------------------------------------
# Analytics with Google Analytics
# https://analytics.google.com
# -----------------------------------------------------------------------------
NEXT_PUBLIC_GOOGLE_ANALYTICS_ID = ""

# -----------------------------------------------------------------------------
# Analytics with OpenPanel
# https://openpanel.dev
# -----------------------------------------------------------------------------
NEXT_PUBLIC_OPENPANEL_CLIENT_ID = ""

# -----------------------------------------------------------------------------
# Payment with Stripe
# https://docs.stripe.com/keys
# -----------------------------------------------------------------------------
STRIPE_PUBLIC_KEY = ""
STRIPE_PRIVATE_KEY = ""
STRIPE_WEBHOOK_SECRET = ""

NEXT_PUBLIC_PAY_SUCCESS_URL = "http://localhost:3000/my-orders"
NEXT_PUBLIC_PAY_FAIL_URL = "http://localhost:3000"
NEXT_PUBLIC_PAY_CANCEL_URL = "http://localhost:3000/#pricing"

NEXT_PUBLIC_LOCALE_DETECTION = "false"

ADMIN_EMAILS = ""
```

## Triển Khai

1. Tạo kho lưu trữ Github

2. Commit mã dự án đã tùy chỉnh vào kho lưu trữ Github

3. Tạo dự án mới trong bảng điều khiển Vercel, nhập kho mã và triển khai bằng một cú nhấp chuột

<img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Cấu hình cài đặt tên miền và chứng chỉ SSL trong bảng điều khiển Vercel

<img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Ra mắt trang web chính thức