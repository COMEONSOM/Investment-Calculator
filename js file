function showLumpSumForm() {
    document.getElementById("lumpSumForm").classList.add("active");
    document.getElementById("sipForm").classList.remove("active");
}

function showSipForm() {
    document.getElementById("sipForm").classList.add("active");
    document.getElementById("lumpSumForm").classList.remove("active");
}

function calculateLumpSum() {
    var lumpSumAmount = parseFloat(document.getElementById("lumpSumAmount").value);
    var lumpSumYears = parseFloat(document.getElementById("lumpSumYears").value);
    var lumpSumInterestRate = parseFloat(document.getElementById("lumpSumInterestRate").value);

    var futureValue = lumpSumAmount * Math.pow(1 + (lumpSumInterestRate / 100), lumpSumYears);
    document.getElementById("result").innerText = "Maturity Amount: " + futureValue.toFixed(2);
}

function calculateSip() {
    var sipMonthlyAmount = parseFloat(document.getElementById("sipMonthlyAmount").value);
    var sipYears = parseFloat(document.getElementById("sipYears").value);
    var sipInterestRate = parseFloat(document.getElementById("sipInterestRate").value);

    var totalInvestment = sipMonthlyAmount * 12 * sipYears;
    var futureValue = totalInvestment * Math.pow(1 + (sipInterestRate / 100), sipYears);
    document.getElementById("result").innerText = "Maturity Amount: " + futureValue.toFixed(2);
}

function clearForm() {
    document.getElementById("lumpSumAmount").value = "";
    document.getElementById("lumpSumYears").value = "";
    document.getElementById("lumpSumInterestRate").value = "";
    document.getElementById("sipMonthlyAmount").value = "";
    document.getElementById("sipYears").value = "";
    document.getElementById("sipInterestRate").value = "";
    document.getElementById("result").innerText = "";
}

function goBack() {
    document.getElementById("lumpSumForm").classList.remove("active");
    document.getElementById("sipForm").classList.remove("active");
}
