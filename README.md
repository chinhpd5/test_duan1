  # Hướng Dẫn Sử Dụng Git cơ bản

  ## 1. Cài đặt Git

  ### Trên Windows:
  Tải Git từ trang chính thức: https://git-scm.com/downloads
  Cài đặt theo hướng dẫn mặc định.


  ## 2. Cấu hình git lần đầu
  Tại Command Prompt(cmd)
  ```bash
    git config --global user.name "Tên của bạn"
    git config --global user.email "email@example.com"
  ```

  Kiểm tra cấu hình:
  ```bash
    git config --list
  ```

  ## 3. Các lệnh git cơ bản

  Khởi tạo git:
  ```bash
    git init
  ```

  Sao chép (clone) một dự án từ GitHub:
  ```bash
    git clone https://github.com/tai-khoan/ten-repo.git
  ```

  Kiểm tra trạng thái:
  ```bash
    git status
  ```

  ### Làm việc với nhánh

  Tạo nhánh mới:
  ```bash
    git branch ten-nhanh
  ```

  Chuyển sang nhánh khác
  ```bash
    git checkout ten-nhanh
  ```
  Tạo và chuyển sang nhánh mới
  ```bash
    git checkout -b ten-nhanh
  ```

  Gộp nhánh
  ```bash
    git checkout main
    git merge ten-nhanh
  ```


  ### Push code (Đẩy code lên github)

  ```bash
    git add .
    git commit -m "message"
    git push origin ten-nhanh
  ```

  ### Pull code (Lấy code từ main)

  ```bash
    git pull origin main
  ```

  ## Demo xử lý merge code và conflict: https://www.loom.com/share/42d709a7b9d4470a89b2b001f90d0fbd