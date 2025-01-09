//Primeira questão resposta: 91

//Segunda Questão

function isFibonacci(num) {
    let a = 0, b = 1;

    while (b <= num) {
        if (b === num) {
            return `${num} pertence à sequência de Fibonacci.`;
        }
        let temp = a + b;
        a = b;
        b = temp;
    }

    return `${num} não pertence à sequência de Fibonacci.`;
}

// Testando com um número:
const numero = 21; 
console.log(isFibonacci(numero));

//Terceira questão

const faturamentoDiario = [1200, 850, 0, 3000, 4100, 0, 700, 1500, 0, 4000]; 

function calcularFaturamento(dados) {
    const diasComFaturamento = dados.filter(valor => valor > 0);
    const menorValor = Math.min(...diasComFaturamento);
    const maiorValor = Math.max(...diasComFaturamento);
    const mediaMensal = diasComFaturamento.reduce((acc, val) => acc + val, 0) / diasComFaturamento.length;
    const diasAcimaMedia = diasComFaturamento.filter(valor => valor > mediaMensal).length;

    return {
        menorValor,
        maiorValor,
        diasAcimaMedia
    };
}

const resultado = calcularFaturamento(faturamentoDiario);
console.log("Menor valor:", resultado.menorValor);
console.log("Maior valor:", resultado.maiorValor);
console.log("Dias acima da média:", resultado.diasAcimaMedia);


//Terceira questão

const faturamentoEstados = {
    SP: 67836.43,
    RJ: 36678.66,
    MG: 29229.88,
    ES: 27165.48,
    Outros: 19849.53
};

function calcularPercentual(faturamento) {
    const total = Object.values(faturamento).reduce((acc, val) => acc + val, 0);
    const percentuais = {};

    for (const estado in faturamento) {
        percentuais[estado] = ((faturamento[estado] / total) * 100).toFixed(2) + '%';
    }

    return percentuais;
}

console.log(calcularPercentual(faturamentoEstados));

//Quarta questão

function inverterString(str) {
    let invertida = "";

    for (let i = str.length - 1; i >= 0; i--) {
        invertida += str[i];
    }

    return invertida;
}

// Testando com uma string:
const texto = "Teste";
console.log("Texto original:", texto);
console.log("Texto invertido:", inverterString(texto));
