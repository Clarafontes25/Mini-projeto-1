
import java.util.Scanner;

class Main{

public static void main(String[] argas) {

Scanner leitor = new Scanner(System.in);
String Escolha;

String Introducao = "Chapeuzinho Vermelho\n\n - Chapeuzinho! Chapeuzinho!, desça as escadas e leve esses doces para a sua vózinha \n - Cheguei mãe, posso pegar um dos doces? \n - Não! pegue esssa cesta e leve para ela, cuidado ao sair, e vá pelo caminho seguro \n\n Ao sair de casa você se depara com dois caminhos, o caminho seguro demora um pouco mais, contudo o caminho perigoso é mais rápido, qual seguir: \n \n - Caminho seguro \n - Caminho perigoso";

String caminho_bom = "Caminho seguro";
String caminho_ruim = "Caminho perigoso";

String final1 =  "Você foi pelo caminho seguro: \n\n - Melhor ir pelo caminho seguro, devagar e sempre! \nVocê chegou no final da tarde na casa da sua vózinha,\n ao chegar lá você foi recebida com um beijo na bochecha e um abraço,\n e sua vózinha te chamou para dormir na casa dela e comer os doces!";

String escolharuim = "Você foi pelo caminho perigoso: \n\n - O que poderia dar de errado, certo? \n Ao andar um pouco, você se depara com um lobo enorme, você vê do seu lado um caminho entre as moitas, contudo cheio de espinhos! \n - O que fazer? se eu for pelos espinhos vou me machucar, mas se eu correr o lobo pode me pegar! \n Qual caminho seguir? \n\n - Moita \n - Correr ";


String ir_moita = "Moita";
String ir_correr = "Correr";


String final2 = "Você decidir ir pela moita! \n\n Os espinhos da moita eram venenos e fazem com que você perca a consciência. Você acorda e ouve uma voz grave\n - Você acordou? eu te achei deitada sobre uma moite de espinhos venenosos,\n sua familia está preocupada com você, vamos para casa! \n Você vê sua mãe e sua vó ao longe, ambas preocupadas, você chora ao perceber que está bem, você decide ser mais cautelosa apartir de hoje! ";

String final3 ="Você decidir correr! \n\n você corre o mais rápido que pode, contudo você não consegue escapar do lobo,\n ele caça você por toda a floresta e finalmente te pega.\n Até hoje, sua vó e sua mãe esperam que um dia você volte da floresta";

System.out.println(Introducao);
Escolha = leitor.nextLine();


      if(Escolha.equals(caminho_ruim))
       {
         System.out.println(escolharuim);
         Escolha = leitor.nextLine();
         if(Escolha.equals(ir_moita))
         {
            System.out.println(final2);
         }else if(Escolha.equals(ir_correr))
         {
            System.out.println(final3);
         }
       }

       if(Escolha.equals(caminho_bom))
       {
        System.out.println(final1);
        Escolha = leitor.nextLine();
       }
      
  }

}
