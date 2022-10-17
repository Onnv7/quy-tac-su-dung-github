## Lệnh git cơ bản
`git init` : khởi tạo git
git add .
git commit -m"<msg>"
git log --oneline : để xem lịch sử commit
git checkout <commit_code> : để quay lại commit trước

git remote add <remote_name> <url> : tạo remote tới repo github

git pull <remote_name> main : pull nhánh main về local

git checkout -b <branch_name> : vừa tạo branch vừa chuyển branch.



git push <remote_name> <branch_name> : 
	đẩy nhánh <branch_name> ở local lên nhánh <branch_name> ở github
	Khi push lần đầu, đồng nghĩa với việc tạo thêm một nhánh <branch_name> ở trên github.


## Quy trình: 
	VD: có một remote tên an_remote
	- Đầu tiên pull nhánh main trên git về mà code: git pull an_remote main
	- Không thao tác trên nhánh MAIN/MASTER ở GITHUB
	- Pull về rồi tạo một branch với tên của mình vd : git checkout -b nguyenvanan
	- Khi làm code xong => dùng git push an_remote nguyenvanan
	- Lên github => chọn nhánh nguyenvanan => nhấp cái link xanh blue có chữ "1 commit ahead" => Button "Create pull request"
	- Ghi title, desc ở ô write rõ ràng => Create pull request
	- Nhắn lên nhóm hoặc nhắn trước khi push lên cũng đc
	- Còn lại để thằng quản lý git xử lý, bấm nhiều quá hư project

## Lưu ý:
	- <remote_name>/<branch_name> : là trỏ đến nhánh <branch_name> trên github mà <remote_name> trỏ đến
	- Luôn kiểm tra có đang ở nhánh của mình không? nếu không thì chuyển sang

## Quản lý git:
	- Một khi có merge thì thông báo lại cho nhóm
	- Nếu có đụng độ trên main khi merge các nhánh từ tv thì tv đó sẽ hỗ trợ giải quyết
