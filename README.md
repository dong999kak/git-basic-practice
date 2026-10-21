# Git Basic Practice

Thực hành vòng đời Git: Working Directory → Staging Area → Repository.

## Các commit chính

- Initial commit: add html and css
- Update html content
- Add javascript file
- Update style and notes

## Ghi chú thực hành

- Ở commit đầu, chỉ index.html và style.css được đưa vào staging; notes.txt vẫn untracked.
- Staging area cho phép chọn chính xác phần thay đổi sẽ nằm trong commit, kể cả khi working directory còn các thay đổi khác.
- git pull là git fetch rồi git merge (hoặc fetch + rebase khi cấu hình pull.rebase).
- git reset --soft: lùi HEAD, giữ nguyên staging area và working directory.
- git reset --mixed: lùi HEAD, giữ working directory, bỏ staging.
- git reset --hard: lùi HEAD và đưa staging/working directory về commit đó; thay đổi chưa commit có thể mất.
- Không nên reset --hard trên commit đã push và được team dùng; ưu tiên git revert để tạo commit đảo ngược, giữ lịch sử chia sẻ an toàn.
