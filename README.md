<h1>biblioteca geração e validação de código EAN</h1>
<hr/>

<p>
<span style='margin-left:10px'>E</span>stá biblioteca tem por finalidade gerar, validar o código e calcular digito verificador o código numérico EAN11, EAN12 e EAN13.
</p>
<a href="https://github.com/wellingtonsluzhotmailcom/ean/raw/master/Ean/dist/Ean.jar">download .jar</a>

<h2>Exemplos de utilização</h2>
<hr/>
<pre>
public static void main(String args[]) {

        try {

            // Gerar código ean13
            System.out.println(Ean.ean13());
            // Gerar código ean12
            System.out.println(Ean.ean12());
            // Gerar código ean11
            System.out.println(Ean.ean11());
            
            // calcula o digito verificador do código ean11
            System.out.println(Ean.calculaDigEan11("78936521589"));
            
            // calcula o digito verificador do código ean12
            System.out.println(Ean.calculaDigEan12("205768415862"));
            
            // calcula o digito verificador do código ean13
            System.out.println(Ean.calculaDigEan13("1808354873641"));
            
            // Válida um código EAN11, EAN 12, EAN13 
            System.out.println(Ean.isEan("789365215891"));
            
        } catch (Exception ex) {
            ex.printStackTrace();
        }

    }
</pre>
