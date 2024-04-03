"# GitTesting" 

Git: Version Control system giúp người sử dụng quản lý các phiên bản của một project

Repository: Nơi lưu trữ project của người dùng

Branch: Nhánh để lưu các thay đổi cho từng user, tránh xảy ra xung đột giữa nhiều người cùng hoạt động trong một dự án

Commit: 1 set các thay đổi

Merge: Hợp nhất file của nhánh nào đó vào nhánh hiện tại

Conflict: Nếu 2 nhánh có các thay đổi ở cùng 1 file và 1 vị trí sẽ xảy ra xung đột, phải giải quyết xung đột thì mới push được

Push: Đưa các thay đổi lên server

Pull: tải các thay đổi có trên server

Checkout: Chọn nhánh nào đó để bắt đầu làm việc

Stash: Lưu các thay đổi vào bộ nhớ tạm

git config --global user.name "TienDat"
-> Set username cho user git

git config --global user.email aityvo987@gmail.com
-> Set email cho user git

git config credential.helper store
-> Lưu thông tin tk, mk user lâu dài

git config credential.helper cache
-> Lưu thông tin tk, mk user ngắn hạn

git config --global alias.s status
-> Lưu tên viết tắt cho các câu lệnh (s cho status)

git clone #something
-> Tải về một Repository dựa trên link #something

git init
-> Khởi tạo Repository cho thư mục hiện tại

git remote add origin #something
-> Gắn file local với link git ở #something, để có thể tuong tác với Repository 

git status
-> Coi tình trạng cập nhật so với bản ở git, các file đã thay đổi so với lần cập nhật gần nhất

git branch #branchname
-> Tạo một branch mới có tên #branchname

git checkout #branchname
-> Chuyển thư mục làm việc sang nhánh có tên #branchname

git add. 
-> Stage tất cả các file

git add ./name-folder
-> Stage file có trong folder có đường dẫn ./name-folder

git reset ./name-folder/...
-> Unstage các file theo đường dẫn

git commit -m "Something"
-> Commit, tức ghi chú cho các file đã thay đổi cho lần cập nhật này

git reset HEAD~1
-> Reset tất cả thay đổi về commit lần trước 

git push
-> Đẩy tất cả những stage file và commit lên git server.

git merge #branchname
-> Merge #branchname vào branch hiện tại

git pull
-> Cập nhật những thay đổi có trong Repository trên server cho tất cả các branch

git stash
-> Bỏ vào ô nhớ tạm thời các thay đổi đã thực hiện trên một branch

git stash pop
-> Lấy ra các thay đổi có trong ô nhớ của một branch

git checkout #branchname ./path-to-file
-> Thay thế file có trong branch hiện tại với file có trên #branchname

git fetch --prune
-> Xoá các branch ở local mà không có trên server