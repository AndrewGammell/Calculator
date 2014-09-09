//Calculator Code Challenge
==========

import java.awt.EventQueue;
import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import javax.swing.JTextField;
import javax.swing.SwingConstants;
import javax.swing.JButton;
import java.awt.Color;
import java.awt.Font;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;


public class CalculatorApp extends JFrame {
	
	boolean sum;
	StringBuilder sbd = new StringBuilder();
    StringBuilder sb = new StringBuilder();
    private String input ="0.0";
    private double input1 =0.0D;
    private String str="";
    private String displayInput ="";
    private double totalInput=0.0D;
    private String operator ;
	private JPanel contentPane;
	private JTextField textFieldDisplay;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					CalculatorApp frame = new CalculatorApp();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public CalculatorApp() {
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100, 100, 418, 389);
		contentPane = new JPanel();
		contentPane.setBackground(Color.RED);
		contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));
		contentPane.setLayout(null);
		setContentPane(contentPane);
		
		textFieldDisplay = new JTextField();
		textFieldDisplay.setFont(new Font("Tahoma", Font.BOLD, 25));
		textFieldDisplay.setHorizontalAlignment(SwingConstants.RIGHT);
		textFieldDisplay.setBounds(10, 11, 382, 43);
		contentPane.add(textFieldDisplay);
		textFieldDisplay.setColumns(10);
		
		JButton button7 = new JButton("7");
		button7.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("7").toString();
                displayInput = sbd.append("7").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button7.setForeground(new Color(255, 0, 0));
		button7.setBackground(new Color(255, 255, 0));
		button7.setFont(new Font("Tahoma", Font.BOLD, 20));
		button7.setBounds(10, 131, 89, 43);
		contentPane.add(button7);
		
		JButton button8 = new JButton("8");
		button8.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("8").toString();
                displayInput = sbd.append("8").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button8.setForeground(new Color(255, 0, 0));
		button8.setBackground(new Color(255, 255, 0));
		button8.setFont(new Font("Tahoma", Font.BOLD, 20));
		button8.setBounds(109, 131, 89, 43);
		contentPane.add(button8);
		
		JButton button9 = new JButton("9");
		button9.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("9").toString();
                displayInput = sbd.append("9").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button9.setForeground(new Color(255, 0, 0));
		button9.setBackground(new Color(255, 255, 0));
		button9.setFont(new Font("Tahoma", Font.BOLD, 20));
		button9.setBounds(208, 131, 89, 43);
		contentPane.add(button9);
		
		JButton button1 = new JButton("1");
		button1.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("1").toString();
                displayInput = sbd.append("1").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button1.setForeground(new Color(255, 0, 0));
		button1.setBackground(new Color(255, 255, 0));
		button1.setFont(new Font("Tahoma", Font.BOLD, 20));
		button1.setBounds(10, 239, 89, 43);
		contentPane.add(button1);
		
		JButton button4 = new JButton("4");
		button4.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("4").toString();
                displayInput = sbd.append("4").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button4.setForeground(new Color(255, 0, 0));
		button4.setBackground(new Color(255, 255, 0));
		button4.setFont(new Font("Tahoma", Font.BOLD, 20));
		button4.setBounds(10, 185, 89, 43);
		contentPane.add(button4);
		
		JButton button5 = new JButton("5");
		button5.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("5").toString();
                displayInput = sbd.append("5").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button5.setForeground(new Color(255, 0, 0));
		button5.setBackground(new Color(255, 255, 0));
		button5.setFont(new Font("Tahoma", Font.BOLD, 20));
		button5.setBounds(109, 185, 89, 43);
		contentPane.add(button5);
		
		JButton button6 = new JButton("6");
		button6.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("6").toString();
                displayInput = sbd.append("6").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button6.setForeground(new Color(255, 0, 0));
		button6.setBackground(new Color(255, 255, 0));
		button6.setFont(new Font("Tahoma", Font.BOLD, 20));
		button6.setBounds(208, 185, 89, 43);
		contentPane.add(button6);
		
		JButton button2 = new JButton("2");
		button2.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("2").toString();
                displayInput = sbd.append("2").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button2.setForeground(new Color(255, 0, 0));
		button2.setBackground(new Color(255, 255, 0));
		button2.setFont(new Font("Tahoma", Font.BOLD, 20));
		button2.setBounds(109, 239, 89, 43);
		contentPane.add(button2);
		
		JButton button3 = new JButton("3");
		button3.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("3").toString();
                displayInput = sbd.append("3").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button3.setForeground(new Color(255, 0, 0));
		button3.setBackground(new Color(255, 255, 0));
		button3.setFont(new Font("Tahoma", Font.BOLD, 20));
		button3.setBounds(208, 239, 89, 43);
		contentPane.add(button3);
		
		JButton button0 = new JButton("0");
		button0.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append("0").toString();
                displayInput = sbd.append("0").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		button0.setForeground(new Color(255, 0, 0));
		button0.setBackground(new Color(255, 255, 0));
		button0.setFont(new Font("Tahoma", Font.BOLD, 20));
		button0.setBounds(10, 293, 89, 43);
		contentPane.add(button0);
		
		JButton buttonDot = new JButton(".");
		buttonDot.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				input = sb.append(".").toString();
                displayInput = sbd.append(".").toString();
                textFieldDisplay.setText(displayInput);
			}
		});
		buttonDot.setForeground(new Color(0, 0, 0));
		buttonDot.setBackground(new Color(0, 191, 255));
		buttonDot.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonDot.setBounds(109, 293, 89, 43);
		contentPane.add(buttonDot);
		
		JButton buttonClear = new JButton("Clear");
		buttonClear.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
               input ="";
               textFieldDisplay.setText(""); 
               input1=0.0D;
               totalInput=0.0D;
               sb.replace(0, sb.length(),str).toString();
               sbd.replace(0, sbd.length(),str).toString();
           }
       });
		buttonClear.setForeground(new Color(0, 0, 0));
		buttonClear.setBackground(new Color(0, 0, 255));
		buttonClear.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonClear.setBounds(307, 77, 89, 43);
		contentPane.add(buttonClear);
		
		JButton buttonPlus = new JButton("+");
		buttonPlus.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {          
                input1 = Double.parseDouble(input);                
                input = sb.replace(0, sb.length(),str).toString();
                displayInput = sbd.append("+").toString();
                textFieldDisplay.setText(displayInput);
			if(totalInput==0){
				totalInput += input1;
			}
                	if(operator=="+"){
                   		 totalInput += input1 ;
                	}else if(operator=="-"){
                		totalInput -= input1;
                	}else if(operator=="*"){
                		totalInput *= input1;
                	}else if(operator=="/"){
                		totalInput /= input1;
                	}else if(operator == "="){
                		totalInput += 0;
                	}
                	textFieldDisplay.setText(displayInput);
                	operator = "+";
            }
        });
		buttonPlus.setForeground(new Color(0, 0, 0));
		buttonPlus.setBackground(new Color(0, 191, 255));
		buttonPlus.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonPlus.setBounds(307, 131, 89, 43);
		contentPane.add(buttonPlus);
		
		JButton buttonMinus = new JButton("\u2212");
		 buttonMinus.addActionListener(new ActionListener() {
	            public void actionPerformed(ActionEvent e) {  	
	                input1 = Double.parseDouble(input);                
	                input = sb.replace(0, sb.length(),str).toString();
	                displayInput = sbd.append("\u2212").toString();
	                textFieldDisplay.setText(displayInput);
	                	if(totalInput==0){
	                		totalInput += input1;
	                	}
	                	if(operator=="+"){
	                    		totalInput += input1 ;
	                	}else if(operator=="-"){
	                		totalInput -= input1;
	                	}else if(operator=="*"){
	                		totalInput *= input1;
	                	}else if(operator=="/"){
	                		totalInput /= input1;
	                	}else if(operator == "="){
	                		totalInput += 0;
	                   	}
	                operator = "-";
	                System.out.println(totalInput);
	            }
	        });
		buttonMinus.setForeground(new Color(0, 0, 0));
		buttonMinus.setBackground(new Color(0, 191, 255));
		buttonMinus.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonMinus.setBounds(307, 185, 89, 43);
		contentPane.add(buttonMinus);
		
		JButton buttonMultiply = new JButton("\u00D7");
		buttonMultiply.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {           
                input1 = Double.parseDouble(input);                
                input = sb.replace(0, sb.length(),str).toString();
                displayInput = sbd.append("\u00D7").toString();
                textFieldDisplay.setText(displayInput);
                if(totalInput==0){
                	totalInput += input1;
                	}
                	if(operator=="+"){
                    totalInput += input1 ;
                	}else if(operator=="-"){
                		totalInput -= input1;
                	}else if(operator=="*"){
                		totalInput *= input1;
                	}else if(operator=="/"){
                		totalInput /= input1;
                	}else if(operator == "="){
                		totalInput += 0;
               	}
                operator = "*";
            }
        });
		buttonMultiply.setForeground(new Color(0, 0, 0));
		buttonMultiply.setBackground(new Color(0, 191, 255));
		buttonMultiply.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonMultiply.setBounds(307, 239, 89, 43);
		contentPane.add(buttonMultiply);
		
		JButton buttonDivide = new JButton("\u00F7");
		buttonDivide.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
            	
                input1 = Double.parseDouble(input);                
                input = sb.replace(0, sb.length(),str).toString();
                displayInput = sbd.append("\u00F7").toString();
                textFieldDisplay.setText(displayInput);
                if(totalInput==0){
                	totalInput += input1;
                	}
                	if(operator=="+"){
                    totalInput += input1 ;
                	}else if(operator=="-"){
                		totalInput -= input1;
                	}else if(operator=="*"){
                		totalInput *= input1;
                	}else if(operator=="/"){
                		totalInput /= input1;
                	} else if(operator == "="){
                		totalInput += 0;
               	}
                operator = "/";  
            }
        });
		buttonDivide.setForeground(new Color(0, 0, 0));
		buttonDivide.setBackground(new Color(0, 191, 255));
		buttonDivide.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonDivide.setBounds(307, 293, 89, 43);
		contentPane.add(buttonDivide);
		
		JButton buttonEquals = new JButton("\u003D");
		buttonEquals.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
            	
            	displayInput = sbd.append("\u003D").toString();
            	input1 = Double.parseDouble(input);
            	if(operator=="+"){
                	totalInput += input1 ;
            	}else if(operator=="-"){
            		totalInput -= input1;
            	}else if(operator=="*"){
            		totalInput *= input1;
            	}else if(operator=="/"){
            		totalInput /= input1;
            	}else if(totalInput == 0){
            		totalInput += input1;	
            	}
            	
		if(totalInput % 1==0){
              displayInput = sbd.append(((int)totalInput)).toString();
		}else{displayInput = sbd.append(String.format("%.2f", totalInput)).toString();
		}
                textFieldDisplay.setText(displayInput);
                operator = "=";
             }
        });
		buttonEquals.setForeground(new Color(0, 0, 0));
		buttonEquals.setBackground(new Color(0, 191, 255));
		buttonEquals.setFont(new Font("Tahoma", Font.BOLD, 20));
		buttonEquals.setBounds(208, 293, 89, 43);
		contentPane.add(buttonEquals);
	}
}
