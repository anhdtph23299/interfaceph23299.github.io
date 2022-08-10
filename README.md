# Interface trong Java
## 1. Đặc điểm của interface : 
- Phương thức trong interface đều trừu tượng, nghĩa là không có thân hàm, và đều có modifier là: public abstract, cho dù bạn có khai báo hay không.
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
- Ví dụ : 
```Java
public interface InterfaceSV  {
    void inRaManHinh();
    void themDoiTuong();
}
```
- Nhìn qua , có vẻ 2 phương thức trong interface Demo có vẻ khác nhau . Tuy nhiên , trong interface hệ thống tự biên dịch và chỉnh sửa theo khung là public abstract + Phương thức . Vì vậy , 2 phương thức trên hoàn toàn giống nhau .
- Khi Một class kế thừa interface , class đó sẽ phải ghi đè phương thức (Override) mà interface đó có : 
```Java
public class SinhVien implements InterfaceSV {

    @Override
    public void inRaManHinh() {
        System.out.println("Đây là phương thức in ra màn hình");
    }

    @Override
    public void themDoiTuong() {
        System.out.println("Đây là phương thức thêm đối tượng");

    }

}
```
## 3. Đa kế thừa trong interface
- Khi học qua về OOP , các bạn đều biết Đối tượng chỉ được đơn kế thừa nhưng 
