// Función para calcular el máximo común divisor (MCD)
function calcularMCD(a, b) {
    a = Math.abs(a); // Considerar el valor absoluto para números negativos
    b = Math.abs(b);
    while (b !== 0) {
        let temp = b;
        b = a % b;
        a = temp;
    }
    return a;
}

// Función para calcular la sumatoria
function calcularSumatoria() {
    const limiteInferior = parseInt(document.getElementById("limiteInferior").value);
    const limiteSuperior = parseInt(document.getElementById("limiteSuperior").value);

    if (isNaN(limiteInferior) || isNaN(limiteSuperior)) {
        document.getElementById("resultado").innerText = "Por favor, ingrese valores válidos.";
        return;
    }

    if (limiteInferior > limiteSuperior) {
        document.getElementById("resultado").innerText = "El límite inferior no puede ser mayor al límite superior.";
        return;
    }

    let sumatoria = 0;
    for (let k = limiteInferior; k <= limiteSuperior; k++) {
        sumatoria += calcularMCD(k, 15);
    }

    document.getElementById("resultado").innerText = `La sumatoria de MCD(k, 15) desde ${limiteInferior} hasta ${limiteSuperior} es: ${sumatoria}`;
}
