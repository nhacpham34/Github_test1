# Github_test1
Tìm hiểu về github cơ bản:
Sơ lược về Git
- Trong Git , Repository(Repo) là một kho chứa, lưu trữ source code của bạn,
có 2 loại repository: 
  + Local Repository: là nơi chứa code ngay trên máy tính của mình
  + Remote Repository: là nơi chứa code trên sever được cung cấp bởi hotting sevice như
  GitHub, GitLab, Bitbucket
- Dùng git config để kết nối Local Repository với Remote Repository(GitHub Account :
  + git version : kiểm tra phiên bản git trên máy tính
  + git config --global user.name ["tên Local"]: tạo tên local repo
  + git config --global user.email ["tên email github"]: link với github account
  + git config --list : dùng để check lại xem mình đã config đúng chưa
- Git Workflow : quy trình xử lý (workflow) trên Git:
Bắt đầu từ Working Derectory(Thư mục làm việc) -> init ->Initalization -> git add ->
Staging Area(Khu vực chuẩn bị) -> git commit (lưu lại bản chụp(snapshot) của những
thay đổi trong Working Directory) -> Local Repository -> git push (đẩy nhưng thay đổi trên
Local Repo(My PC) lên Remote Repo (GitHub) -> GitHub
- 10 lệnh Git cơ bản mà developer cần phải biết:
 *1. Lệnh Git Init
  + git init: Tạo local repo trên máy tính của mình
   (init = Initialize : Khởi chạy or khởi tạo)
  + Tạo remote repository trên GitHub
  + git reomote add origin [link liên kết]: Liên kết local repository với GitHub repo
 *2. Lệnh Git Clone:Clone(tải) a Remote Repo on GitHub to Local PC
  + git clone [GitHub_Repo_URL]
 *3. Git Add: lưu những thay đổi vào trong Staging Area
  + git add [file muốn add]
 *4. Git Commit: lưu lại Snapshots(ảnh chụp) của những sự thay đổi trong working Directory
  + git commit -m ["descriptive message (mô tả sự thay đổi"]
  + git commit --amend -m "amend descriptive message": thay đổi đoạn mô tả mới
 *5. Git Push: Uploads tất cả các commit trong local repo lên remote repo (github)
  + git push origin [branch-name(tên nhánh)]: master
 *6. Git Status: dùng để check trạng thái trong working directory( thư mục làm việc) and 
 staging area (Khu vực chuẩn bị)
  + git status
 *7. Git Diff: dùng để xem các thay đổi của các commit với nhau
  + git diff [mã cũ] [mã mới]
 *8. Git Log: List ra các commit đã thực hiện trên current branch(nhánh hiện tại)
  + git log
  + git log --oneline : hiển thị mỗi commit trên một dòng
 *9. Git Reset: Remove the specified file from the staging area, but leave the working
 directory unchanged ( xóa file đã add vào khu vực chuẩn bị)
  + git reset <file>
  + git reset [--soft | --mixed | --hard | --merge | --keep] <commit>: tìm hiểu thêm
 *10. Git Fetch & Pull: Synchronize(đồng bộ hóa) local repo với remote repo
  + git fetch: fetch(lấy) những thay đổi mới nhất trên remote repo xuông local repo
  + git pull: pull(kéo, tải xuống) những thay đổi và update nhưng thay đổi vào local repo.
