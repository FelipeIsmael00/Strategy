<?PHP

namespace Tests\Feature;

use PHPUnit\Framework\TestCase;
use App\Discount\Strategies\SeasonalDiscount;

class SeasonalDiscountTest extends TestCase
{
    // Método de teste para validar a regra de desconto para pedidos acima de 300.
    public function testAplicaDescontoDe45ParaPedidoAcimaDe300()
    {
        // Instancia a classe que contém a regra de desconto.
        $discount = new SeasonalDiscount();

        // Executa o cálculo do desconto para um pedido de 350,00.
        $resultado = $discount->calculate(350.00);

        // Verifica se o resultado retornado é igual a 45,00.
        // Se não for, o teste falhará.
        $this->assertEquals(45.00, $resultado);
    }

    public function testAplicaDescontoDe10ParaPedidoAte300()
    {
        $discount = new SeasonalDiscount();

        $resultado = $discount->calculate(80.00);

        $this->assertEquals(10.00, $resultado);
    }
}
