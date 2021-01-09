# GUI4
ex4
import java.awt.Color;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;

public class Ex8 implements ActionListener{

	public JPanel createContentPane()
	{
		JPanel GUI=new JPanel();
		GUI.setLayout(null);
		
		JPanel yazilar=new JPanel();
		yazilar.setLayout(null);
		yazilar.setLocation(10,0);
        yazilar.setSize(250,30);
        GUI.add(yazilar);
        
		JLabel down=new JLabel("volumn down");
		down.setForeground(Color.black);
		down.setLocation(0,0);
		down.setSize(100,30);
		down.setHorizontalAlignment(0);
		yazilar.add(down);
		
		JLabel up=new JLabel("volumn up");
		up.setForeground(Color.black);
		up.setLocation(90,0);
		up.setSize(100,30);
		up.setHorizontalAlignment(0);
		yazilar.add(up);
	    
		JPanel cubuklar=new JPanel();
		cubuklar.setLayout(null);
		cubuklar.setLocation(10,20);
		cubuklar.setSize(225,150);
		GUI.add(cubuklar);
		
		
		
	 JPanel birinci=new JPanel();
	 birinci.setBackground(Color.black);
	 birinci.setLocation(10,140);
	 birinci.setSize(10,10);
	 cubuklar.add(birinci);
	 
	 JPanel ikinci=new JPanel();
	 ikinci.setBackground(Color.black);
	 ikinci.setLocation(25,130);
	 ikinci.setSize(10,20);
	 cubuklar.add(ikinci);
	 
	 JPanel ucuncu=new JPanel();
	 ucuncu.setBackground(Color.black);
	 ucuncu.setLocation(40,120);
	 ucuncu.setSize(10,30);
	 cubuklar.add(ucuncu);
	 
	 JPanel dorduncu=new JPanel();
	 dorduncu.setBackground(Color.black);
	 dorduncu.setLocation(55,110);
	 dorduncu.setSize(10,40);
	 cubuklar.add(dorduncu);
	 
	 JPanel besinci=new JPanel();
	 besinci.setBackground(Color.black);
	 besinci.setLocation(70,100);
	 besinci.setSize(10,50);
	 cubuklar.add(besinci);
	 
	 JPanel altıncı=new JPanel();
	 altıncı.setBackground(Color.black);
	 altıncı.setLocation(85,90);
	 altıncı.setSize(10,60);
	 cubuklar.add(altıncı);
	 
	 JPanel yedinci=new JPanel();
	 yedinci.setBackground(Color.black);
	 yedinci.setLocation(100,80);
	 yedinci.setSize(10,70);
	 cubuklar.add(yedinci);
	 
	 JPanel sekizinci=new JPanel();
	 sekizinci.setBackground(Color.black);
	 sekizinci.setLocation(115,70);
	 sekizinci.setSize(10,80);
	 cubuklar.add(sekizinci);
	 
	 JPanel dokuzuncu=new JPanel();
	 dokuzuncu.setBackground(Color.black);
	 dokuzuncu.setLocation(130,60);
	 dokuzuncu.setSize(10,90);
	 cubuklar.add(dokuzuncu);
	 
	 JPanel onuncu=new JPanel();
	 onuncu.setBackground(Color.black);
	 onuncu.setLocation(145,50);
	 onuncu.setSize(10,100);
	 cubuklar.add(onuncu);
	 
	 JPanel butonlar=new JPanel();
	 butonlar.setLayout(null);
	 butonlar.setLocation(10,200);
	 butonlar.setSize(225,50);
	 GUI.add(butonlar);
	 
	 JButton azalt =new JButton(" - ");
	 azalt.setLocation(25,0);
	 azalt.setSize(50,30);
	 azalt.addActionListener(this);//implements ettik
	 butonlar.add(azalt);
	 
	 JButton arttır =new JButton(" + ");
	 arttır.setLocation(100,0);
	 arttır.setSize(50,30);
	 arttır.addActionListener(this);
	 butonlar.add(arttır);
	 
	 return GUI;
	}
	public static void main(String args[])
	{
		JFrame frame=new JFrame("**SES SİSTEMİ**");
		JFrame.setDefaultLookAndFeelDecorated(true);
		Ex8 demo=new Ex8()	;
		frame.setContentPane(demo.createContentPane());
		frame.setSize(225,300);
		frame.setVisible(true);
	}
	@Override
	public void actionPerformed(ActionEvent e) {
		// TODO Auto-generated method stub
		
	}
}
