<?PHP

namespace App\Discount\Strategies;

// Importa a interface DiscountStrategy, que a classe SeasonalDiscount vai implementar.
use App\Discount\DiscountStrategy;

// Define a classe SeasonalDiscount, que implementa a interface DiscountStrategy.
class SeasonalDiscount implements DiscountStrategy
{
// Método que pega o contrato feito na interface DiscountStrategy e calcula o desconto com base no valor do pedido.
    public function calculate(float $orderAmount): float
    {
// Essa linha usa o operador ternário, se o valor for 300 ou mais, retorna um desconto fixo de 45.00, caso contrário, retorna um desconto fixo menor, de 10.00.
        return $orderAmount > 300 ? 45.00 : 10.00;
    }
}
