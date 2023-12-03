package View;

import javax.swing.*;

public class Demo {
    public static void main(String[] args) {
        JFrame jf = new JFrame();
        jf.setSize(600, 400); // Nhập tỉ lệ khung hình.
        jf.setTitle("DEMO");   // Điền tên của cửa sổ.
        jf.setLocation(430,130); // Set hiển thị cửa sổ trên màn hình.
        jf.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE); // thoát ra khỏi trường trình khi đóng JFrame.
        jf.setVisible(true);  //Lệnh cho phép hiển thị (True = Hiện,  False = )

    }
}


package View;

import javax.swing.*;

public class MyWindow extends JFrame {

    public MyWindow()
    {

    }
    public void showIt()
    {
        this.setVisible(true);
        this.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
    public void showIt(String title){
        this.setTitle(title);
        this.setVisible(true);
    }
    public void showIt(String title, int width, int height)
    {
        this.setTitle(title);
        this.setSize(500, 400);
        this.setVisible(true);
    }

}
import View.MyWindow;

public class Main {
    public static void main(String[] args) {
        MyWindow m1 = new MyWindow();
        m1.showIt();

        MyWindow m2 = new MyWindow();
        m2.showIt("WINDOW2");

        MyWindow m3 = new MyWindow();
        m3.showIt("WINDOW3", 500, 400);
    }
}
