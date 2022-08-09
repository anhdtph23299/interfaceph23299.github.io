# Interface trong Java
## 1. Đặc điểm của interface : 
- Bất cứ gì trong interface đều trừu tượng, nghĩa là không có thân hàm, và đều có modifier là: public abstract, cho dù bạn có khai báo hay không.
- Interface không có hàm khởi tạo (constructor).
- Interface không phải là một đối tượng . 
- Khi một Class kế thừa interface , Class đó phải ghi đè (Override) lại các thuộc tích trong interface đó . 
## 2. Interface khác Class về gì ? 
- Bạn không thể khởi tạo một interface.
- Một interface không chứa bất cứ hàm Contructor nào.
- Tất cả các phương thức của interface đều là abstract.
- Một interface không thể chứa một trường nào trừ các trường vừa static và final.
- Một interface không thể kế thừa từ lớp, nó được triển khai bởi một lớp.
- Một interface có thể kế thừa từ nhiều interface khác.
