h2. [Frontend Mentor] Blog Preview Card – Vue 3

h3. Mục tiêu

Xây dựng Blog Preview Card bằng Vue 3 + Vite theo Figma/design Frontend Mentor; giao diện responsive, có trạng thái hover/focus và đáp ứng các yêu cầu accessibility cơ bản.

h3. Tài liệu tham khảo

* Challenge: https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS
* Figma: sử dụng file thiết kế đã được cung cấp cho bài tập.
* Starter: assets/images, assets/fonts, style-guide.md.

h3. Yêu cầu chức năng và giao diện

* Hiển thị một blog card gồm: illustration, category (Learning), ngày xuất bản (21 Dec 2023), tiêu đề (HTML & CSS foundations), mô tả và thông tin tác giả (avatar, Greg Hooper).
* Giao diện bám sát thiết kế desktop (1440px), mobile (375px) và active states.
* Responsive từ 320px đến màn hình lớn; không tràn ngang, card giữ khoảng cách hợp lý với mép màn hình.
* Có hover và keyboard focus rõ ràng cho mọi phần tử tương tác thực sự.
* Sử dụng màu và font Figtree theo style guide; weights 500 và 800.
* Sử dụng asset từ starter; đường dẫn ảnh hoạt động trong production build.

h3. Yêu cầu kỹ thuật

* Vue 3 + Vite; SCSS; component BlogPreviewCard nhận dữ liệu qua props.
* Không cần Vue Router hoặc Pinia cho bài tập một trang.
* Semantic HTML phù hợp (main, article, heading, time); alt hợp lý cho ảnh.
* Nếu tiêu đề là link, dùng URL hợp lệ và hỗ trợ focus-visible; không dùng link giả.
* Bảo đảm tương phản màu, thứ tự đọc và khả năng sử dụng bằng bàn phím.
* Không hardcode đường dẫn src/assets dạng chuỗi trong object; dùng import asset hoặc public URL.

h3. Acceptance criteria (Definition of Done)

* UI bám sát thiết kế desktop/mobile và active states.
* Hiển thị đầy đủ dữ liệu card, ảnh/font tải đúng trên local và production.
* Responsive ổn định từ 320px, không tràn ngang.
* Các phần tử tương tác có hover/focus; semantic và keyboard accessibility cơ bản đạt yêu cầu.
* Production build thành công, link deploy truy cập được.
* Repository và README sẵn sàng để submit.