# Programa-IMC "Em java"
package ExerciciosConceitosBasicos;
import java.util.Locale;
import javax.swing.JOptionPane;

public class Imc {
	public static void main(String[] args) {
		
		Locale.setDefault(Locale.US);
		
		String nomeEntrada = JOptionPane.showInputDialog(" Digite seu nome : ");
		String EntradaPeso = JOptionPane.showInputDialog(" Digite seu peso : ");
		String EntradaAltura = JOptionPane.showInputDialog(" Digite sua altura : ");
		
		
		double peso = Double.parseDouble(EntradaPeso);
		double Altura = Double.parseDouble(EntradaAltura);
		double Altura2 = (Altura * Altura);
		double Imc = peso / Altura2 ;
		String nome = nomeEntrada;
		
		//JOptionPane.showMessageDialog(null, Imc); função pra imprimir na tela
		
	            	JOptionPane.showMessageDialog(null, nome + " seu Imc é --> " +  Imc);
		           // System.out.printf("Seu Imc é --> %.2f " , Imc);
				if (Imc < 18.5)
					JOptionPane.showMessageDialog(null, " Abaixo do peso ideal, vamos melhorar!");
		            //System.out.println ("Abaixo do peso ideal, vamos melhorar!");
		        else
		            if ((Imc > 18.5) &&(Imc <24.9))
		            	JOptionPane.showMessageDialog(null, " Voce esta no peso ideal, parabens!");
		                //System.out.println ("Voce esta no peso ideal, parabens!");
		        else
		                if ((Imc > 25.0)&& (Imc <29.9))
		                	JOptionPane.showMessageDialog(null, " Voce está com excesso de peso, vamos melhorar!");
		                   // System.out.println("Voce está com excesso de peso, vamos melhorar!");
		        else
		                    if ((Imc > 30.0) && (Imc <34.9))
		                    	JOptionPane.showMessageDialog(null, "Obesidade Classe I, cuidado!");	
		                    //System.out.println("Obesidade Classe I, cuidado!");
		        else
		                        if ((Imc > 35.0) && (Imc <39.9))
		                        	JOptionPane.showMessageDialog(null, "Obesidade Classe II, ainda temos como mudar isso!");
		                            //System.out.println ("Obesidade Classe II, ainda temos como mudar isso!");
		        else 
		                            if (Imc >= 40)
		                            	JOptionPane.showMessageDialog(null, "Obesidade Classe III, procure ajuda, nada está perdido!");
		                                //System.out.println ("Obesidade Classe III, procure ajuda, nada está perdido!");
		                   
		                            
				JOptionPane.showMessageDialog(null, "Obrigado :-)");
		       // System.out.println("Obrigado :)");
					
								
	}

}
