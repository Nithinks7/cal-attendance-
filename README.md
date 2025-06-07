* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
    min-height: 100vh;
    padding: 2rem;
}

.container {
    max-width: 1000px;
    margin: 0 auto;
}

h1 {
    text-align: center;
    color: #2c3e50;
    margin-bottom: 2rem;
    font-size: 2.5rem;
}

h1 i {
    margin-right: 0.5rem;
    color: #3498db;
}

.calculator-card {
    background: white;
    border-radius: 15px;
    padding: 2rem;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    margin-bottom: 2rem;
}

.input-section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin-bottom: 2rem;
}

.input-group {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

label {
    color: #2c3e50;
    font-weight: 500;
}

input {
    padding: 0.8rem;
    border: 2px solid #e0e0e0;
    border-radius: 8px;
    font-size: 1rem;
    transition: border-color 0.3s ease;
}

input:focus {
    outline: none;
    border-color: #3498db;
}

.calculate-btn {
    background: #3498db;
    color: white;
    border: none;
    padding: 1rem;
    border-radius: 8px;
    font-size: 1.1rem;
    cursor: pointer;
    transition: background 0.3s ease, transform 0.3s ease;
    grid-column: 1 / -1;
}

.calculate-btn:hover {
    background: #2980b9;
    transform: translateY(-2px);
}

.results-section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.5rem;
    margin-top: 2rem;
}

.result-card {
    background: #f8f9fa;
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
    transition: transform 0.3s ease;
}

.result-card:hover {
    transform: translateY(-5px);
}

.result-card h3 {
    color: #2c3e50;
    margin-bottom: 0.5rem;
    font-size: 1.1rem;
}

.result-value {
    font-size: 1.5rem;
    font-weight: bold;
    color: #3498db;
}

.info-section {
    background: white;
    border-radius: 15px;
    padding: 2rem;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

.info-section h2 {
    color: #2c3e50;
    margin-bottom: 1rem;
}

.info-section ol {
    padding-left: 1.5rem;
    color: #2c3e50;
}

.info-section li {
    margin-bottom: 0.5rem;
    line-height: 1.6;
}

/* Status Colors */
.status-good {
    color: #2ecc71 !important;
}

.status-warning {
    color: #f1c40f !important;
}

.status-danger {
    color: #e74c3c !important;
}

/* Responsive Design */
@media screen and (max-width: 768px) {
    body {
        padding: 1rem;
    }

    h1 {
        font-size: 2rem;
    }

    .calculator-card {
        padding: 1.5rem;
    }

    .input-section {
        grid-template-columns: 1fr;
    }

    .results-section {
        grid-template-columns: 1fr;
    }
} 
