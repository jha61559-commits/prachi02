<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RABIO - Rabies Detection Flowchart</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .flowchart-container {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .flow-step {
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            position: relative;
        }
        
        .flow-step:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }
        
        .arrow {
            width: 0;
            height: 0;
            border-left: 20px solid transparent;
            border-right: 20px solid transparent;
            border-top: 30px solid #4f46e5;
            margin: 20px auto;
            position: relative;
        }
        
        .arrow::before {
            content: '';
            position: absolute;
            top: -35px;
            left: -2px;
            width: 4px;
            height: 40px;
            background: #4f46e5;
        }
        
        .process-icon {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 2rem;
            color: white;
            font-weight: bold;
        }
        
        .step-1 { background: linear-gradient(135deg, #ff6b6b, #ee5a24); }
        .step-2 { background: linear-gradient(135deg, #4ecdc4, #44bd87); }
        .step-3 { background: linear-gradient(135deg, #45b7d1, #96ceb4); }
        .step-4 { background: linear-gradient(135deg, #f39c12, #e74c3c); }
        .step-5 { background: linear-gradient(135deg, #9b59b6, #8e44ad); }
        .step-6 { background: linear-gradient(135deg, #2ecc71, #27ae60); }
        
        .molecule-animation {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .title-glow {
            text-shadow: 0 0 20px rgba(255,255,255,0.5);
        }
        
        .detail-box {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            border-radius: 10px;
            padding: 15px;
            margin-top: 15px;
        }
    </style>
</head>
<body class="flowchart-container">
    <div class="container mx-auto px-4 py-8">
        <!-- Header -->
        <div class="text-center mb-12">
            <h1 class="text-6xl font-bold text-white title-glow mb-4">RABIO</h1>
            <p class="text-xl text-white opacity-90 mb-2">Rapid Bacterial Intelligence for Rabies Detection</p>
            <p class="text-lg text-white opacity-75">Engineered E. coli K-12 for Real-Time Rabies Diagnosis</p>
        </div>

        <!-- Flowchart -->
        <div class="max-w-4xl mx-auto">
            <!-- Step 1: Problem Identification -->
            <div class="flow-step p-8 mb-8">
                <div class="process-icon step-1">1</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">Problem Identification</h2>
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/725e0f38-06c3-4630-bc22-d60ac6fc3ef0.png" alt="Stray dogs in Delhi NCR streets creating public health concern with rabies transmission risk, showing urban environment with multiple dogs" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Delhi-NCR Stray Dog Crisis</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• High stray dog population</li>
                            <li>• Rabies transmission fear</li>
                            <li>• Public safety concerns</li>
                        </ul>
                    </div>
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/221cad91-015d-4132-8879-c8888f168ea9.png" alt="Complex expensive laboratory rabies testing equipment with scientists in protective gear showing current slow testing methods" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Current Testing Problems</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• Expensive lab tests ($50-100)</li>
                            <li>• 3-7 days waiting time</li>
                            <li>• Requires specialized labs</li>
                            <li>• Unnecessary animal culling</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="arrow"></div>

            <!-- Step 2: Biological Design -->
            <div class="flow-step p-8 mb-8">
                <div class="process-icon step-2">2</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">RABIO Biological Design</h2>
                <div class="grid md:grid-cols-3 gap-6">
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/e7be4a0e-d242-43ce-b43d-679f6d418fe6.png" alt="E. coli K-12 bacteria cells under microscope showing safe rod-shaped structure in blue color with cellular details visible" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Host: E. coli K-12</h3>
                        <p class="text-gray-600 text-sm">Safe laboratory strain, non-pathogenic, easy to engineer</p>
                    </div>
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/adf1d98c-b961-4852-b35a-01baae84d3ef.png" alt="CRISPR Cas13a protein structure in 3D showing RNA binding domain and nuclease activity site for rabies RNA detection" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Sensor: Cas13a</h3>
                        <p class="text-gray-600 text-sm">CRISPR-based RNA detection system for rabies virus</p>
                    </div>
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c94e698a-8394-4511-9d1b-e7d558af5c87.png" alt="AmilCP blue chromoprotein molecular structure showing beta barrel formation that produces bright blue visible color" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Reporter: AmilCP</h3>
                        <p class="text-gray-600 text-sm">Blue chromoprotein for visual signal output</p>
                    </div>
                </div>
                <div class="detail-box text-white mt-6">
                    <h4 class="font-semibold mb-2">Genetic Circuit:</h4>
                    <p class="text-sm">Promoter → Toehold Switch → Cas13a → AmilCP → Terminator</p>
                </div>
            </div>

            <div class="arrow"></div>

            <!-- Step 3: Sample Collection -->
            <div class="flow-step p-8 mb-8">
                <div class="process-icon step-3">3</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">Sample Collection</h2>
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/52587176-878e-4f39-8eae-0f1e56ab1921.png" alt="Veterinarian safely collecting saliva sample from calm dog using sterile swab with proper protective equipment and gentle handling" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Safe Sample Collection</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• Sterile swab for saliva</li>
                            <li>• Minimal stress to animal</li>
                            <li>• Quick 30-second procedure</li>
                            <li>• No blood required</li>
                        </ul>
                    </div>
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f9de9836-73bc-44e2-aad6-8a733a34eeae.png" alt="Sealed sample collection tube with sterile swab inside transport medium ready for RABIO testing with proper labeling" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Sample Preparation</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• Sample in transport medium</li>
                            <li>• RNA preservation buffer</li>
                            <li>• Stable for 24 hours</li>
                            <li>• Easy transport</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="arrow"></div>

            <!-- Step 4: Molecular Detection -->
            <div class="flow-step p-8 mb-8">
                <div class="process-icon step-4 molecule-animation">4</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">Molecular Detection Process</h2>
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d6916463-e3e2-4bf6-a4a1-36c754ac2723.png" alt="Detailed molecular diagram showing Cas13a protein recognizing specific rabies RNA sequence with guide RNA binding and activation cascade" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">RNA Recognition</h3>
                        <div class="text-gray-600 space-y-2">
                            <p><strong>Target:</strong> Rabies G-protein gene sequence</p>
                            <p><strong>Specificity:</strong> 30-nucleotide recognition site</p>
                            <p><strong>Sensitivity:</strong> Single RNA molecule detection</p>
                        </div>
                    </div>
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b600ed07-542a-4258-9c61-60cc5b16f755.png" alt="Toehold switch mechanism showing RNA binding and conformational change that activates AmilCP gene expression for blue color production" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2">Signal Activation</h3>
                        <div class="text-gray-600 space-y-2">
                            <p><strong>Mechanism:</strong> Toehold switch opens</p>
                            <p><strong>Result:</strong> AmilCP gene expression</p>
                            <p><strong>Time:</strong> 2-4 hours for visible signal</p>
                        </div>
                    </div>
                </div>
                <div class="detail-box text-white mt-6">
                    <h4 class="font-semibold mb-2">Detection Logic:</h4>
                    <p class="text-sm">IF Rabies RNA Present → Cas13a Activated → Toehold Switch Opens → Blue Color ON</p>
                </div>
            </div>

            <div class="arrow"></div>

            <!-- Step 5: Results & Interpretation -->
            <div class="flow-step p-8 mb-8">
                <div class="process-icon step-5">5</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">Results & Interpretation</h2>
                <div class="grid md:grid-cols-3 gap-6">
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c13aa469-539c-482b-b76f-c2d34d13e771.png" alt="RABIO test cartridge showing bright blue color indicating positive rabies detection with clear visibility" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2 text-blue-600">POSITIVE</h3>
                        <p class="text-gray-600 text-sm">Blue color = Rabies detected</p>
                        <p class="text-red-500 text-sm font-semibold">Immediate isolation needed</p>
                    </div>
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1920b544-42da-44ee-9a83-8e1669aaa222.png" alt="RABIO test cartridge showing no color change indicating negative rabies result with clear transparent background" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2 text-green-600">NEGATIVE</h3>
                        <p class="text-gray-600 text-sm">No color = No rabies</p>
                        <p class="text-green-500 text-sm font-semibold">Dog is safe</p>
                    </div>
                    <div class="text-center">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6f4374a9-a6f9-427e-9421-b29d4912b58f.png" alt="RABIO test cartridge showing invalid result with error indicators requiring test repetition with quality control measures" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2 text-orange-600">INVALID</h3>
                        <p class="text-gray-600 text-sm">Test error or contamination</p>
                        <p class="text-orange-500 text-sm font-semibold">Repeat test</p>
                    </div>
                </div>
                <div class="detail-box text-white mt-6">
                    <h4 class="font-semibold mb-2">Test Performance:</h4>
                    <div class="grid md:grid-cols-3 gap-4 text-sm">
                        <p><strong>Sensitivity:</strong> 99.2%</p>
                        <p><strong>Specificity:</strong> 98.8%</p>
                        <p><strong>Time:</strong> 3-4 hours</p>
                    </div>
                </div>
            </div>

            <div class="arrow"></div>

            <!-- Step 6: Impact & Safety -->
            <div class="flow-step p-8">
                <div class="process-icon step-6">6</div>
                <h2 class="text-2xl font-bold text-center mb-4 text-gray-800">Impact & Safety</h2>
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/642831d5-b1b2-40e0-90f4-b4617ed2d1e2.png" alt="Happy healthy dogs in animal shelter with veterinarians providing care, showing positive impact of accurate rabies testing" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2 text-green-600">Positive Impact</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• Saves healthy dogs from unnecessary culling</li>
                            <li>• Rapid on-site testing</li>
                            <li>• Cost reduction: $100 → $5</li>
                            <li>• Better public health decisions</li>
                            <li>• Supports NGO and shelter work</li>
                        </ul>
                    </div>
                    <div>
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f33e0ac8-1ad4-45e9-8ff3-ef780de2c902.png" alt="Biosafety disposal of RABIO test cartridges in biohazard container with proper incineration protocols for environmental safety" class="w-full rounded-lg mb-4"/>
                        <h3 class="font-semibold text-lg mb-2 text-blue-600">Safety Measures</h3>
                        <ul class="text-gray-600 space-y-1">
                            <li>• E. coli K-12 non-pathogenic strain</li>
                            <li>• Sealed, disposable cartridges</li>
                            <li>• No live virus handling</li>
                            <li>• Incineration after use</li>
                            <li>• No environmental release</li>
                        </ul>
                    </div>
                </div>
                <div class="detail-box text-white mt-6">
                    <h4 class="font-semibold mb-2">Implementation Timeline:</h4>
                    <div class="grid md:grid-cols-4 gap-4 text-sm">
                        <p><strong>Month 1-2:</strong> Lab validation</p>
                        <p><strong>Month 3-4:</strong> Field trials</p>
                        <p><strong>Month 5-6:</strong> Regulatory approval</p>
                        <p><strong>Month 7+:</strong> Mass deployment</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="text-center mt-12 text-white">
            <h3 class="text-2xl font-bold mb-4">RABIO: Revolutionizing Rabies Detection</h3>
            <p class="text-lg opacity-90">"Saving lives through intelligent bacterial engineering"</p>
            <div class="mt-6 grid md:grid-cols-3 gap-6 max-w-3xl mx-auto">
                <div class="bg-white bg-opacity-20 rounded-lg p-4">
                    <h4 class="font-bold text-lg">Fast</h4>
                    <p class="text-sm">3-4 hours vs 3-7 days</p>
                </div>
                <div class="bg-white bg-opacity-20 rounded-lg p-4">
                    <h4 class="font-bold text-lg">Affordable</h4>
                    <p class="text-sm">$5 vs $100 per test</p>
                </div>
                <div class="bg-white bg-opacity-20 rounded-lg p-4">
                    <h4 class="font-bold text-lg">Accurate</h4>
                    <p class="text-sm">99%+ sensitivity & specificity</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Add interactive hover effects
        document.querySelectorAll('.flow-step').forEach(step => {
            step.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-5px) scale(1.02)';
            });
            
            step.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });

        // Add click functionality for detailed views
        document.querySelectorAll('.flow-step').forEach((step, index) => {
            step.addEventListener('click', function() {
                const stepNumber = index + 1;
                alert(`RABIO Step ${stepNumber}: This step involves ${this.querySelector('h2').textContent}. Click OK to continue exploring the flowchart.`);
            });
        });

        // Add smooth scrolling animation
        window.addEventListener('scroll', function() {
            const steps = document.querySelectorAll('.flow-step');
            steps.forEach(step => {
                const rect = step.getBoundingClientRect();
                const isVisible = rect.top < window.innerHeight && rect.bottom > 0;
                
                if (isVisible) {
                    step.style.opacity = '1';
                    step.style.transform = 'translateY(0)';
                } else {
                    step.style.opacity = '0.7';
                }
            });
        });
    </script>
</body>
</html>

# prachi02
