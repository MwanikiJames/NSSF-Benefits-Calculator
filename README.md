<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NSSF Benefits Calculator</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #1e3a8a 0%, #1e40af 100%);
        }
        .result-card {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
        }
        .result-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header -->
    <header class="gradient-bg text-white">
        <div class="container mx-auto px-4 py-8">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <h1 class="text-3xl font-bold flex items-center">
                        <i data-feather="shield" class="mr-2"></i> NSSF Benefits Calculator
                    </h1>
                    <p class="mt-2 text-blue-100">Calculate your National Social Security Fund benefits with ease</p>
                </div>
                <div class="flex items-center space-x-4">
                    <a href="#" class="px-4 py-2 bg-white text-blue-800 rounded-lg font-medium hover:bg-blue-100 transition">Login</a>
                    <a href="#" class="px-4 py-2 border border-white rounded-lg font-medium hover:bg-blue-700 transition">Register</a>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="gradient-bg text-white py-16">
        <div class="container mx-auto px-4">
            <div class="max-w-3xl mx-auto text-center">
                <h2 class="text-4xl font-bold mb-6" data-aos="fade-up">Estimate Your Retirement Benefits</h2>
                <p class="text-xl text-blue-100 mb-8" data-aos="fade-up" data-aos-delay="100">
                    Our calculator helps you understand how much you can expect to receive from NSSF based on your contributions.
                </p>
                <a href="#calculator" class="inline-block px-8 py-3 bg-yellow-400 text-blue-900 font-bold rounded-lg hover:bg-yellow-300 transition" data-aos="fade-up" data-aos-delay="200">
                    Calculate Now <i data-feather="arrow-down" class="ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Calculator Section -->
    <section id="calculator" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto">
                <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                    <div class="md:flex">
                        <!-- Input Form -->
                        <div class="md:w-1/2 p-8">
                            <h3 class="text-2xl font-bold text-gray-800 mb-6">Enter Your Details</h3>
                            
                            <div class="mb-6">
                                <label class="block text-gray-700 font-medium mb-2">Monthly Salary (KES)</label>
                                <input type="number" id="salary" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="e.g. 50000">
                            </div>
                            
                            <div class="mb-6">
                                <label class="block text-gray-700 font-medium mb-2">Years of Contribution</label>
                                <input type="number" id="years" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="e.g. 20">
                            </div>
                            
                            <div class="mb-6">
                                <label class="block text-gray-700 font-medium mb-2">Current Age</label>
                                <input type="number" id="age" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="e.g. 35">
                            </div>
                            
                            <button id="calculate-btn" class="w-full py-3 bg-blue-600 text-white font-bold rounded-lg hover:bg-blue-700 transition flex items-center justify-center">
                                <i data-feather="calculator" class="mr-2"></i> Calculate Benefits
                            </button>
                        </div>
                        
                        <!-- Results Display -->
                        <div class="md:w-1/2 bg-gray-50 p-8">
                            <h3 class="text-2xl font-bold text-gray-800 mb-6">Your Estimated Benefits</h3>
                            
                            <div id="results" class="space-y-6">
                                <div class="text-center py-12">
                                    <i data-feather="bar-chart-2" class="mx-auto text-gray-400 w-12 h-12 mb-4"></i>
                                    <p class="text-gray-500">Enter your details to see your estimated NSSF benefits</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works Section -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">How NSSF Benefits Work</h2>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-6 rounded-xl shadow-md" data-aos="fade-up">
                    <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mb-4">
                        <i data-feather="dollar-sign" class="text-blue-600"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Contribution Rates</h3>
                    <p class="text-gray-600">Employees contribute 6% of their salary while employers contribute 6%, making a total of 12% monthly contribution.</p>
                </div>
                
                <div class="bg-white p-6 rounded-xl shadow-md" data-aos="fade-up" data-aos-delay="100">
                    <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mb-4">
                        <i data-feather="clock" class="text-blue-600"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Vesting Period</h3>
                    <p class="text-gray-600">You must contribute for at least 10 years to qualify for full retirement benefits from NSSF.</p>
                </div>
                
                <div class="bg-white p-6 rounded-xl shadow-md" data-aos="fade-up" data-aos-delay="200">
                    <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mb-4">
                        <i data-feather="percent" class="text-blue-600"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Interest Rates</h3>
                    <p class="text-gray-600">NSSF provides competitive interest rates on your contributions, compounded annually.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Frequently Asked Questions</h2>
            
            <div class="max-w-3xl mx-auto space-y-4">
                <div class="border border-gray-200 rounded-lg overflow-hidden" data-aos="fade-up">
                    <button class="faq-question w-full px-6 py-4 text-left font-medium text-gray-700 bg-gray-50 hover:bg-gray-100 transition flex justify-between items-center">
                        <span>What is the minimum contribution period to qualify for benefits?</span>
                        <i data-feather="chevron-down" class="transform transition-transform duration-300"></i>
                    </button>
                    <div class="faq-answer px-6 py-4 bg-white hidden">
                        <p class="text-gray-600">You need to contribute for at least 10 years to qualify for full retirement benefits. However, you can access partial benefits if you contribute for a shorter period.</p>
                    </div>
                </div>
                
                <div class="border border-gray-200 rounded-lg overflow-hidden" data-aos="fade-up" data-aos-delay="100">
                    <button class="faq-question w-full px-6 py-4 text-left font-medium text-gray-700 bg-gray-50 hover:bg-gray-100 transition flex justify-between items-center">
                        <span>Can I access my NSSF benefits before retirement age?</span>
                        <i data-feather="chevron-down" class="transform transition-transform duration-300"></i>
                    </button>
                    <div class="faq-answer px-6 py-4 bg-white hidden">
                        <p class="text-gray-600">Yes, you can access your benefits under special circumstances such as permanent disability, emigration, or terminal illness.</p>
                    </div>
                </div>
                
                <div class="border border-gray-200 rounded-lg overflow-hidden" data-aos="fade-up" data-aos-delay="200">
                    <button class="faq-question w-full px-6 py-4 text-left font-medium text-gray-700 bg-gray-50 hover:bg-gray-100 transition flex justify-between items-center">
                        <span>How often are benefits paid out?</span>
                        <i data-feather="chevron-down" class="transform transition-transform duration-300"></i>
                    </button>
                    <div class="faq-answer px-6 py-4 bg-white hidden">
                        <p class="text-gray-600">Retirement benefits are paid as a lump sum. However, you can opt for monthly payments under certain conditions.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 flex items-center">
                        <i data-feather="shield" class="mr-2"></i> NSSF Calculator
                    </h3>
                    <p class="text-gray-400">Helping you plan for a secure retirement through accurate NSSF benefit calculations.</p>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Home</a></li>
                        <li><a href="#calculator" class="text-gray-400 hover:text-white transition">Calculator</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">About NSSF</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Resources</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">NSSF Act</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Contribution Rates</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Retirement Planning</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">FAQs</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Contact Us</h4>
                    <ul class="space-y-2">
                        <li class="flex items-center text-gray-400"><i data-feather="mail" class="mr-2"></i> info@nssfcalculator.com</li>
                        <li class="flex items-center text-gray-400"><i data-feather="phone" class="mr-2"></i> +254 700 000 000</li>
                        <li class="flex items-center text-gray-400"><i data-feather="map-pin" class="mr-2"></i> Nairobi, Kenya</li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
                <p>© 2023 NSSF Benefits Calculator. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize AOS animations
        AOS.init({
            duration: 800,
            easing: 'ease-in-out',
            once: true
        });

        // Initialize feather icons
        feather.replace();

        // FAQ toggle functionality
        document.querySelectorAll('.faq-question').forEach(question => {
            question.addEventListener('click', () => {
                const answer = question.nextElementSibling;
                const icon = question.querySelector('i');
                
                // Toggle answer visibility
                answer.classList.toggle('hidden');
                
                // Rotate icon
                if (answer.classList.contains('hidden')) {
                    icon.style.transform = 'rotate(0deg)';
                } else {
                    icon.style.transform = 'rotate(180deg)';
                }
            });
        });

        // Calculator functionality
        document.getElementById('calculate-btn').addEventListener('click', calculateBenefits);

        function calculateBenefits() {
            const salary = parseFloat(document.getElementById('salary').value);
            const years = parseFloat(document.getElementById('years').value);
            const age = parseFloat(document.getElementById('age').value);
            
            // Validate inputs
            if (isNaN(salary) || isNaN(years) || isNaN(age) || salary <= 0 || years <= 0 || age <= 0) {
                alert('Please enter valid positive numbers for all fields');
                return;
            }
            
            // Calculate benefits (simplified calculation - real NSSF calculations are more complex)
            const monthlyContribution = salary * 0.12; // 12% total contribution (6% employee + 6% employer)
            const totalContributions = monthlyContribution * 12 * years;
            
            // Apply simple interest (real NSSF uses compound interest with varying rates)
            const interestRate = 0.08; // 8% annual interest (example)
            const interestEarned = totalContributions * interestRate * years;
            
            const totalBenefits = totalContributions + interestEarned;
            
            // Format as currency
            const formatter = new Intl.NumberFormat('en-KE', {
                style: 'currency',
                currency: 'KES',
                minimumFractionDigits: 2
            });
            
            // Display results
            document.getElementById('results').innerHTML = `
                <div class="result-card bg-white p-6 rounded-lg border border-gray-200">
                    <h4 class="font-bold text-gray-700 mb-2">Total Contributions</h4>
                    <p class="text-2xl font-bold text-blue-600">${formatter.format(totalContributions)}</p>
                    <p class="text-sm text-gray-500 mt-1">Over ${years} years</p>
                </div>
                
                <div class="result-card bg-white p-6 rounded-lg border border-gray-200">
                    <h4 class="font-bold text-gray-700 mb-2">Interest Earned</h4>
                    <p class="text-2xl font-bold text-green-600">${formatter.format(interestEarned)}</p>
                    <p class="text-sm text-gray-500 mt-1">At ~${(interestRate * 100).toFixed(1)}% p.a.</p>
                </div>
                
                <div class="result-card bg-blue-50 p-6 rounded-lg border border-blue-200">
                    <h4 class="font-bold text-gray-700 mb-2">Estimated Total Benefits</h4>
                    <p class="text-3xl font-bold text-blue-700">${formatter.format(totalBenefits)}</p>
                    <p class="text-sm text-gray-500 mt-1">At retirement age ${age + years}</p>
                </div>
                
                <div class="text-center pt-4">
                    <p class="text-sm text-gray-500">Note: This is an estimate. Actual NSSF benefits may vary based on official rates and regulations.</p>
                </div>
            `;
            
            // Replace icons in new content
            feather.replace();
        }
    </script>
</body>
</html>
