import org.junit.jupiter.api.Test;

import static org.junit.jupiter.api.Assertions.assertTrue;
import static org.junit.jupiter.api.Assertions.fail;

public class InicialTest {

    private Calculadora calculadora = new Calculadora();

    @Test
    public void testSomarDoisNumeros() {
        int resultado = calculadora.somar(2, 3);
        if (resultado != 5) {
            fail("2 + 3 deveria ser 5, mas foi " + resultado);
        }

        resultado = calculadora.somar(0, 0);
        if (resultado != 0) {
            fail("0 + 0 deveria ser 0, mas foi " + resultado);
        }

        resultado = calculadora.somar(2, -3);
        if (resultado != -1) {
            fail("2 + (-3) deveria ser -1, mas foi " + resultado);
        }
    }

    @Test
    public void testSubtrairDoisNumeros() {
        int resultado = calculadora.subtrair(3, 2);
        if (resultado != 1) {
            fail("3 - 2 deveria ser 1, mas foi " + resultado);
        }

        resultado = calculadora.subtrair(2, 7);
        if (resultado != -5) {
            fail("2 - 7 deveria ser -5, mas foi " + resultado);
        }

        resultado = calculadora.subtrair(0, 0);
        if (resultado != 0) {
            fail("0 - 0 deveria ser 0, mas foi " + resultado);
        }
    }

    @Test
    public void testMultiplicarDoisNumeros() {
        int resultado = calculadora.multiplicar(2, 3);
        if (resultado != 6) {
            fail("2 * 3 deveria ser 6, mas foi " + resultado);
        }

        resultado = calculadora.multiplicar(0, 5);
        if (resultado != 0) {
            fail("0 * 5 deveria ser 0, mas foi " + resultado);
        }

        resultado = calculadora.multiplicar(2, -4);
        if (resultado != -8) {
            fail("2 * (-4) deveria ser -8, mas foi " + resultado);
        }
    }

    @Test
    public void testDividirDoisNumeros() {
        double resultado = calculadora.dividir(4, 2);
        if (Math.abs(resultado - 2.0) > 0.0001) {
            fail("4 / 2 deveria ser 2.0, mas foi " + resultado);
        }

        resultado = calculadora.dividir(1, 2);
        if (Math.abs(resultado - 0.5) > 0.0001) {
            fail("1 / 2 deveria ser 0.5, mas foi " + resultado);
        }

        resultado = calculadora.dividir(-6, 2);
        if (Math.abs(resultado - (-3.0)) > 0.0001) {
            fail("-6 / 2 deveria ser -3.0, mas foi " + resultado);
        }
    }

    @Test
    public void testDividirPorZero() {
        try {
            calculadora.dividir(5, 0);
            fail("Deveria ter lançado ArithmeticException");
        } catch (ArithmeticException e) {
            // Teste passou - exceção foi lançada como esperado
            assertTrue(true);
        }
    }

    @Test
    public void testSomarArray() {
        int resultado = calculadora.somar(new int[]{1, 2, 3, 4});
        if (resultado != 10) {
            fail("Soma do array deveria ser 10, mas foi " + resultado);
        }

        resultado = calculadora.somar(new int[]{});
        if (resultado != 0) {
            fail("Soma do array vazio deveria ser 0, mas foi " + resultado);
        }

        resultado = calculadora.somar(new int[]{2, -3, -4});
        if (resultado != -5) {
            fail("Soma do array deveria ser -5, mas foi " + resultado);
        }
    }

    @Test
    public void testSubtrairArray() {
        int resultado = calculadora.subtrair(new int[]{10, 5, 3});
        if (resultado != 2) {
            fail("Subtração do array deveria ser 2, mas foi " + resultado);
        }

        resultado = calculadora.subtrair(new int[]{});
        if (resultado != 0) {
            fail("Subtração do array vazio deveria ser 0, mas foi " + resultado);
        }

        resultado = calculadora.subtrair(new int[]{5, 10, 15});
        if (resultado != -20) {
            fail("Subtração do array deveria ser -20, mas foi " + resultado);
        }
    }

    @Test
    public void testMultiplicarArray() {
        int resultado = calculadora.multiplicar(new int[]{2, 3, 4});
        if (resultado != 24) {
            fail("Multiplicação do array deveria ser 24, mas foi " + resultado);
        }

        resultado = calculadora.multiplicar(new int[]{});
        if (resultado != 0) {
            fail("Multiplicação do array vazio deveria ser 0, mas foi " + resultado);
        }

        resultado = calculadora.multiplicar(new int[]{2, -3, 4});
        if (resultado != -24) {
            fail("Multiplicação do array deveria ser -24, mas foi " + resultado);
        }
    }

    @Test
    public void testDividirArray() {
        double resultado = calculadora.dividir(new int[]{8, 2, 2});
        if (Math.abs(resultado - 2.0) > 0.0001) {
            fail("Divisão do array deveria ser 2.0, mas foi " + resultado);
        }

        resultado = calculadora.dividir(new int[]{8, 2, 2, 2, 2});
        if (Math.abs(resultado - 0.5) > 0.0001) {
            fail("Divisão do array deveria ser 0.5, mas foi " + resultado);
        }

        resultado = calculadora.dividir(new int[]{});
        if (Math.abs(resultado - 0.0) > 0.0001) {
            fail("Divisão do array vazio deveria ser 0.0, mas foi " + resultado);
        }
    }

    @Test
    public void testDividirArrayPorZero() {
        try {
            calculadora.dividir(new int[]{10, 2, 0});
            fail("Deveria ter lançado ArithmeticException");
        } catch (ArithmeticException e) {
            // Teste passou - exceção foi lançada como esperado
            assertTrue(true);
        }
    }
}
