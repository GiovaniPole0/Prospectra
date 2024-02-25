# Prospectra
Staking Anticipation Platform

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleERC20 {
    string public name = "Prospectra";
    string public symbol = "SPEC";
    uint8 public decimals = 18;
    uint256 public totalSupply;
    mapping(address => uint256) public balanceOf;

    event Transfer(address indexed from, address indexed to, uint256 value);

    constructor(uint256 initialSupply) {
        totalSupply = initialSupply * (10 ** uint256(decimals));
        balanceOf[msg.sender] = totalSupply;
        emit Transfer(address(0), msg.sender, totalSupply);
    }

    function transfer(address to, uint256 value) external returns (bool) {
        require(to != address(0), "Transfer to the zero address");
        require(balanceOf[msg.sender] >= value, "Insufficient balance");

        balanceOf[msg.sender] -= value;
        balanceOf[to] += value;
        emit Transfer(msg.sender, to, value);
        return true;
    }
}

Bem-vindo (a) à Prospectra

Imagine ter a capacidade de antecipar seus ativos de staking travados em qualquer criptomoeda, obtendo liquidez instantânea e lucro. Além disso, troque suas stablecoins por Alticoins sem pagar taxas. Sim, você leu certo! Ao emprestar seus USDC, USDT ou DAI para quem quer sair de staking travados para fazer lucro você receberá de volta juros na criptomoeda em que decidiu fazer emprestimo.

Para quem quer sair do Staking travado

Com a Prospectra, os usuários podem antecipar seus ativos de staking travados em qualquer criptomoeda e receber USDC, USDT ou DAI instantaneamente, mantendo a flexibilidade para otimizar seus portfólios conforme necessário. Por exemplo, imagine que um investidor tenha $10.000 em Polkadot e, repentinamente, o valor dessa criptomoeda sobe para $13.000. Nesse cenário, ao utilizar nossa plataforma, o investidor pode realizar seu lucro imediato. Após assinar o contrato inteligente, ele receberá aproximadamente $12.200, levando em consideração as taxas pagas ao provedor de empréstimo de USDC, USDT e DAI, e para a própria Prospectra.

Recompensas de Staking após assinar com a Prospectra
Os usuários que optarem por trocar seus Tokens em staking travado irão receber todas as recompensas acumuladas durante o período em que suas criptomoedas estavam em staking, até a data em que assinam o contrato inteligente.

Após a aceitação do contrato, as criptomoedas continuarão em staking de acordo com o período de desbloqueio da blockchain equestão.

No entanto, o valor do staking após a assinatura do contrato, ao fim do período determinado, será direcionado para a plataforma, enquanto o usuário receberá todas as recompensas acumuladas. Por exemplo, se o usuário deixou seus tokens em staking por 100 dias, ele receberá os ganhos correspondentes a esse período. Os lucros acumulados após a assinatura do contrato serão retidos pela plataforma.

Para quem quer emprestar USDC, USDT e DAI em troca de juros em criptomoedas

 

O valor recebido é calculado com base na taxa de juros e no dia do empréstimo, proporcionando uma vantagem adicional. Ao optar pela nossa plataforma, os usuários evitam as taxas associadas à troca de seus USDC, USDT ou DAI por outra criptomoeda em exchanges. Por exemplo, se trocarem 100 USDC em uma exchange, acabam recebendo menos do que 100 Dólares da criptomoeda que fez a conversao, devido às taxas envolvidas. No entanto, na Prospectra, ao emprestar 100 USDC, eles podem receber de volta um valor maior, como 130 USDC na criptomoeda acordada. Isso oferece um benefício significativo em comparação com as trocas tradicionais.
Emprestar para a PAAS:
 

​

Os usuários emprestam seus USDC, USDT ou DAI para a PAAS em troca de juros na criptomoeda que decidiram emprestar através do contrato inteligente.

Cálculo de Retorno:
 

Exemplo 1: Polkadot (28 dias): O retorno é calculado com base na taxa de juros acordada e no preço da moeda no dia em que concordaram com o empréstimo.
Exemplo 2: Ethereum (11 dias): Da mesma forma, o retorno é calculado com base na taxa de juros e no dia do empréstimo.
Exemplo 3: Matic (8 dias): Os usuários receberão a quantidade acordada de Matic, calculada com base na taxa de juros e no dia do empréstimo.

Negocie mais de 50 criptomoedas

Atendimento ao cliente 24/7

Plataformas DeFi integradas

Descentralizada

decentralized financ (15).jpg
Geração de Receita com a  Prospectra
​Taxas de Juros: Após a aceitação do contrato, as criptomoedas continuarão em staking de acordo com o período de desbloqueio da blockchain em questão. O valor do staking após a assinatura do contrato, ao fim do período determinado, será direcionado para a plataforma, enquanto o usuário receberá todas as recompensas acumuladas. Os lucros acumulados após a assinatura do contrato serão retidos pela plataforma.

Taxas de Assinatura: Ao assinarem contratos com a Prospectra para lucrar, os usuários também podem gerar receita para a plataforma por meio das taxas de assinatura cobradas.

Gestão de Ativos: As criptomoedas recebidas em taxas e após saírem de staking podem ser guardadas até uma alta do mercado ou vendidas, funcionando como uma exchanger e gerando lucros adicionais para a Prospectra.

