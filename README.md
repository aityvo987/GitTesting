"# GitTesting" 
<div id="header" align="center">
  <img src="https://i.imgur.com/c7iirLS.jpg" width="100"/>
    <div id="badges">
        <a href="your-linkedin-URL">
            <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
        </a>
        <a href="your-youtube-URL">
            <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
        </a>
        <a href="your-twitter-URL">
            <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
        </a>
    </div>
    <h1>Halo</h1>
</div>

---

### :black_nib: About Me :


- :pencil2: Git: Version Control system giúp người sử dụng quản lý các phiên bản của một project

- :pencil2: Repository: Nơi lưu trữ project của người dùng

- :pencil2: Branch: Nhánh để lưu các thay đổi cho từng user, tránh xảy ra xung đột giữa nhiều người cùng hoạt động trong một dự án

- :pencil2: Commit: 1 set các thay đổi

- :pencil2: Merge: Hợp nhất file của nhánh nào đó vào nhánh hiện tại

- :pencil2: Rebase: Lấy những thay đổi của nhánh target để đưa vào nhánh hiện tại

- :pencil2: Cherry-pick: Giống merge nhưng chỉ lấy lần commit gần nhất của merge

- :pencil2: Conflict: Nếu 2 nhánh có các thay đổi ở cùng 1 file và 1 vị trí sẽ xảy ra xung đột, phải giải quyết xung đột thì mới push được

- :pencil2: Push: Đưa các thay đổi lên server

- :pencil2: Pull: tải các thay đổi có trên server

- :pencil2: Checkout: Chọn nhánh nào đó để bắt đầu làm việc

- :pencil2: Stash: Lưu các thay đổi vào bộ nhớ tạm

git config --global user.name "TienDat"
:arrow_right:  Set username cho user git

git config --global user.email aityvo987@gmail.com
:arrow_right:  Set email cho user git

git config credential.helper store
:arrow_right: Lưu thông tin tk, mk user lâu dài

git config credential.helper cache
:arrow_right:  Lưu thông tin tk, mk user ngắn hạn

git config --global alias.s status
:arrow_right:  Lưu tên viết tắt cho các câu lệnh (s cho status)

git clone #something
:arrow_right:  Tải về một Repository dựa trên link #something

git init
:arrow_right:  Khởi tạo Repository cho thư mục hiện tại

git remote add origin #something
:arrow_right:  Gắn file local với link git ở #something, để có thể tuong tác với Repository 

git status
:arrow_right:  Coi tình trạng cập nhật so với bản ở git, các file đã thay đổi so với lần cập nhật gần nhất

git branch #branchname
:arrow_right:  Tạo một branch mới có tên #branchname

git checkout #branchname
:arrow_right:  Chuyển thư mục làm việc sang nhánh có tên #branchname

git add. 
:arrow_right:  Stage tất cả các file

git add ./name-folder
:arrow_right:  Stage file có trong folder có đường dẫn ./name-folder

git reset ./name-folder/...
:arrow_right:  Unstage các file theo đường dẫn

git commit -m "Something"
:arrow_right:  Commit, tức ghi chú cho các file đã thay đổi cho lần cập nhật này

git reset HEAD~1
:arrow_right:  Reset tất cả thay đổi về commit lần trước 

git push
:arrow_right:  Đẩy tất cả những stage file và commit lên git server.

git merge #branchname
:arrow_right:  Merge #branchname vào branch hiện tại

git pull
:arrow_right:  Cập nhật những thay đổi có trong Repository trên server cho tất cả các branch

git stash
:arrow_right:  Bỏ vào ô nhớ tạm thời các thay đổi đã thực hiện trên một branch

git stash pop
:arrow_right:  Lấy ra các thay đổi có trong ô nhớ của một branch

git checkout #branchname ./path-to-file
:arrow_right:  Thay thế file có trong branch hiện tại với file có trên #branchname

git fetch --prune

:arrow_right:  Xoá các branch ở local mà không có trên server

git rebase main
:arrow_right:  Giống merge nhưng chỉ ghi đè những thay đổi có trong branch main

git cherry branch-X
:arrow_right:  giống merge nhưng chỉ lấy commit gần nhất của nhánh X để merge lên nhánh hiện tại

test Cherry
