# README

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/490c8239-a3db-497c-a269-b5ee8c9e52a1)

`EHCTF{tôi_đã_hiểu}`

# FOR101

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/06987382-63b7-4c32-981b-e5d27799e5c4)

* sau khi tải file thì mình thấy có 3 folder của 3 địa chỉ ip
* đề bài chỉ ra rằng mã độc ở địa chỉ ip 10.1.108.139 nên mình tìm trong folder đó
* mình thử tìm trong lịch sử duyệt web chrome

![Screenshot 2024-04-27 171522](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/8683b6b0-0ff9-451f-9396-d619a6555e62)

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/0610aa48-c237-4e91-b0ab-136ce98cbc9e)

* user này đã tải file setup.exe tại địa chỉ lạ http://45.77.246.183/bin/

`EHCTF{http://45.77.246.183/bin/setup.exe}`

# FOR102

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/660f1e9b-dcc5-445b-8fd3-068896ae1d5f)

* tại table downloads trên db browser mình đã tìm thấy đường dẫn lưu file setup.exe

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/430a222c-5ce3-4c30-9db5-cbaf76cee0f1)

* đầu tiên mình nghĩ là time này

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/09599b29-2579-471f-8304-76355eac9099)

* tuy nhiên, đây chỉ là thời gian tải xuống của file
* mình nhớ rằng file prefetch lưu trữ cache của file bao gồm cả số lần chạy và thời gian của lần chạy đó
* mình tìm thấy file SETUP.EXE-43E91D36.pf trong folder Prefetch
* dùng PECmd.exe để mở file

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/2c336123-00bf-4904-a5e4-857617835c31)

* file setup.exe này chạy 1 lần duy nhất vào thời gian 2022-10-05 15:10:51

`EHCTF{c:\users\lat\downloads\setup.exe_2022-10-05 15:10:51}`

# FOR103: 

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/60645c79-c4f8-43b4-a61b-7a77edbe4bd9)

* Mình search được bài này https://superuser.com/questions/1052541/how-can-i-get-a-history-of-running-processes
* mình đã thử tìm kiếm trong file Security.evtx xem có process nào lạ không

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/45c3d719-6add-4759-80ce-0df9b4c9d07f)

* sau khi lướt một lúc lâu theo time bắt đầu từ ngày 06/10 thì mình tìm thấy một file hydra.exe với đường dẫn lạ c:\users\lat\appdata\local\temp\hy\hydra.exe

`EHCTF{c:\users\lat\appdata\local\temp\hy\hydra.exe}`

# FOR104

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/88cef4ad-1c1a-43b6-bee3-b61d1aa171ca)

# FOR105

![ảnh](https://github.com/LDV-SpaceK/EHCTF2024/assets/151914246/f4bd58be-9532-4461-b5e1-b8ba5dcd6152)

* mình đi tìm

















