<!DOCTYPE html>
<html>
<head>
    <title>Antibiotic Stewardship Audit</title>
</head>
<body>
    <h1>Antibiotic Stewardship Audit</h1>

    <!-- Section 1: Patient Particulars -->
    <h2>Section 1: Patient Particulars</h2>
    <form id="patientForm">
        <label for="crNumber">CR Number:</label>
        <input type="number" id="crNumber" name="crNumber" required><br>

        <label for="caseNumber">Case Number:</label>
        <input type="number" id="caseNumber" name="caseNumber" required><br>

        <label for="status">Status:</label>
        <select id="status" name="status">
            <option value="RIP">RIP</option>
            <option value="Discharge/LAMA">Discharge/LAMA</option>
            <option value="shifted to ward">Shifted to Ward</option>
        </select><br>

        <label for="admissionDate">Date of Admission:</label>
        <input type="date" id="admissionDate" name="admissionDate" required><br>

        <label for="icuEntryDate">Date of ICU entry:</label>
        <input type="date" id="icuEntryDate" name="icuEntryDate" required><br>

        <label for="finalDiagnosis">Final Diagnosis:</label>
        <input type="text" id="finalDiagnosis" name="finalDiagnosis" required><br>

        <label for="infectiveEtiology">Infective Etiology:</label>
        <input type="checkbox" id="infectiveEtiology" name="infectiveEtiology" value="yes"> Yes
        <input type="checkbox" id="infectiveEtiology" name="infectiveEtiology" value="no"> No<br>

        <label for="centralLine">Central/HD Line:</label>
        <input type="number" id="centralLine" name="centralLine"><br>

        <label for="ventilator">Ventilator:</label>
        <input type="number" id="ventilator" name="ventilator"><br>

        <label for="catheter">Catheter:</label>
        <input type="number" id="catheter" name="catheter"><br>

        <label for="tlc">TLC:</label>
        <input type="number" id="tlc" name="tlc"><br>

        <label for="crp">CRP:</label>
        <input type="number" id="crp" name="crp"><br>

        <label for="creatinine">Creatinine:</label>
        <input type="number" id="creatinine" name="creatinine"><br>
    </form>

    <!-- Section 2: Antibiotic Details -->
    <h2>Section 2: Antibiotic Details</h2>
    <div id="antibiotics">
        <!-- Antibiotic Details Template -->
        <div class="antibiotic-entry">
            <label for="antibiotic">Antibiotic:</label>
            <select class="antibiotic" name="antibiotic">
                <option value="antibiotic1">Antibiotic 1</option>
                <option value="antibiotic2">Antibiotic 2</option>
                <!-- Add more antibiotic options here -->
            </select><br>

            <label for="route">Route:</label>
            <select class="route" name="route">
                <option value="IV">IV</option>
                <option value="IM">IM</option>
                <option value="oral">Oral</option>
                <option value="nebulization">Nebulization</option>
                <option value="topical">Topical</option>
                <option value="rectal">Rectal</option>
            </select><br>

            <label for="frequency">Frequency:</label>
            <select class="frequency" name="frequency">
                <option value="OD">OD</option>
                <option value="BD">BD</option>
                <option value="TDS">TDS</option>
                <option value="QID">QID</option>
            </select><br>

            <label for="dose">Dose:</label>
            <input type="number" class="dose" name="dose">
            <select class="dose-unit" name="dose-unit">
                <option value="g">g</option>
                <option value="mg">mg</option>
                <!-- Add more dose unit options here -->
            </select><br>

            <label for="duration">Duration:</label>
            <input type="number" class="duration" name="duration"><br>

            <label for="indication">Indication:</label>
            <select class="indication" name="indication">
                <option value="empirical">Empirical</option>
                <option value="prophylactic">Prophylactic</option>
                <option value="definitive">Definitive</option>
            </select><br>

            <label for="definitive-indication">Definitive Indication:</label>
            <input type="text" class="definitive-indication" name="definitive-indication"><br>

            <label for="stewardship-issue">Stewardship Issue:</label>
            <input type="checkbox" class="stewardship-issue" name="stewardship-issue" value="not-indicated"> Not Indicated
            <input type="checkbox" class="stewardship-issue" name="stewardship-issue" value="wrong-dose"> Wrong Dose
            <input type="checkbox" class="stewardship-issue" name="stewardship-issue" value="renal-adjustment"> Renal Adjustment Not Done
                        <input type="checkbox" class="stewardship-issue" name="stewardship-issue" value="overlapping-coverage"> Overlapping Coverage
        </div>
    </div>

    <button type="button" id="addAntibiotic">Add Antibiotic</button><br>

    <label for="moreAntibiotics">More Antibiotics:</label>
    <input type="checkbox" id="moreAntibiotics" name="moreAntibiotics"><br>

    <button type="submit">Save Entry to Google Sheets</button>
   
    <!-- Include the Google Sheets API client library script -->
<script src="https://apis.google.com/js/api.js"></script>

<script>
    // JavaScript code for handling form submissions and Google Sheets integration
    document.getElementById("patientForm").addEventListener("submit", function (event) {
        event.preventDefault(); // Prevent the default form submission behavior

        // Collect and structure the form data as needed
        const patientData = {
            crNumber: document.getElementById("crNumber").value,
            caseNumber: document.getElementById("caseNumber").value,
            status: document.getElementById("status").value,
            admissionDate: document.getElementById("admissionDate").value,
            icuEntryDate: document.getElementById("icuEntryDate").value,
            finalDiagnosis: document.getElementById("finalDiagnosis").value,
            infectiveEtiology: document.querySelector('input[name="infectiveEtiology"]:checked').value,
            centralLine: document.getElementById("centralLine").value,
            ventilator: document.getElementById("ventilator").value,
            catheter: document.getElementById("catheter").value,
            tlc: document.getElementById("tlc").value,
            crp: document.getElementById("crp").value,
            creatinine: document.getElementById("creatinine").value,
        };

        const antibioticsData = [];
        const antibioticEntries = document.querySelectorAll(".antibiotic-entry");

        antibioticEntries.forEach(function (entry) {
            const antibioticData = {
                antibiotic: entry.querySelector(".antibiotic").value,
                route: entry.querySelector(".route").value,
                frequency: entry.querySelector(".frequency").value,
                dose: entry.querySelector(".dose").value,
                doseUnit: entry.querySelector(".dose-unit").value,
                duration: entry.querySelector(".duration").value,
                indication: entry.querySelector(".indication").value,
                definitiveIndication: entry.querySelector(".definitive-indication").value,
                stewardshipIssues: Array.from(entry.querySelectorAll(".stewardship-issue:checked")).map((checkbox) => checkbox.value),
            };
            antibioticsData.push(antibioticData);
        });

        const completeData = {
            patientData: patientData,
            antibioticsData: antibioticsData,
        };

        // Initialize the Google Sheets API
        gapi.load("client", function () {
            gapi.client.init({
                apiKey: 'AIzaSyDw3EEUUgkgbVnujAjSMtWLLQASVpNoKcc', // Replace with your Google API key
                discoveryDocs: ["https://sheets.googleapis.com/$discovery/rest?version=v4"],
            }).then(function () {
                // Google API client is loaded and ready

                // Replace with your Google Sheets spreadsheet ID and sheet name
                const spreadsheetId = "1iDNTzLYR-TG13fn_pq4nBqeYWPFFLumD9W3nUuQt7jA";
                const sheetName = "Sheet1"; // Change to your sheet name

                // Prepare the data for the request
                const values = [
                    [
                        completeData.patientData.crNumber,
                        completeData.patientData.caseNumber,
                        completeData.patientData.status,
                        completeData.patientData.admissionDate,
                        completeData.patientData.icuEntryDate,
                        completeData.patientData.finalDiagnosis,
                        completeData.patientData.infectiveEtiology,
                        completeData.patientData.centralLine,
                        completeData.patientData.ventilator,
                        completeData.patientData.catheter,
                        completeData.patientData.tlc,
                        completeData.patientData.crp,
                        completeData.patientData.creatinine,
                    ],
                    // ... (Add more rows for antibioticsData as needed)
                ];

                // Make the request to update Google Sheets
                gapi.client.sheets.spreadsheets.values.append({
                    spreadsheetId: spreadsheetId,
                    range: sheetName,
                    valueInputOption: "RAW",
                    insertDataOption: "INSERT_ROWS",
                    values: values,
                }).then(function(response) {
                    // Data successfully appended to Google Sheets
                    console.log("Data saved to Google Sheets:", response);

                    // Optionally, reset the form after successful submission
                    document.getElementById("patientForm").reset();
                }, function(error) {
                    // Handle error
                    console.error("Error saving data to Google Sheets:", error);
                });
            });
        });
    });
</script>


</body>
</html>