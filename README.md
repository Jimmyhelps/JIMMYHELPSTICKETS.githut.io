<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Official Ticket Sales | Manchester United vs Arsenal | Old Trafford</title>
    <style>
        :root {
            --red: #DA291C;
            --dark-red: #9E1C12;
            --green: #28a745;
            --dark-green: #218838;
            --gold: #FFD700;
            --gray: #333333;
            --light-gray: #f5f5f5;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            color: var(--gray);
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://www.manutd.com/assets/images/hero-images/old-trafford-hero.jpg');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .logo {
            max-width: 150px;
            margin-bottom: 1rem;
        }
        
        h1 {
            margin: 0;
            font-size: 2.5rem;
            color: white;
        }
        
        .match-info {
            background-color: var(--red);
            color: white;
            padding: 1rem;
            margin: 1rem 0;
            border-radius: 5px;
            display: inline-block;
        }
        
        .stadium-map {
            width: 100%;
            max-width: 800px;
            margin: 2rem auto;
            border: 3px solid var(--red);
        }
        
        .sections-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .section {
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 1rem;
            position: relative;
        }
        
        .section.sold-out {
            opacity: 0.7;
        }
        
        .section.sold-out::after {
            content: "SOLD OUT";
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: var(--red);
            color: white;
            padding: 0.5rem 1rem;
            font-weight: bold;
            border-radius: 5px;
            font-size: 1.2rem;
        }
        
        .section h3 {
            margin-top: 0;
            color: var(--red);
        }
        
        .section-location {
            display: inline-block;
            padding: 0.3rem 0.6rem;
            background-color: var(--dark-red);
            color: white;
            border-radius: 3px;
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
        }
        
        .price {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--dark-red);
            margin: 0.5rem 0;
        }
        
        .btn {
            display: inline-block;
            color: white;
            padding: 0.8rem 1.5rem;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background-color 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }
        
        .btn-get-now {
            background-color: var(--green);
        }
        
        .btn-get-now:hover {
            background-color: var(--dark-green);
        }
        
        .btn-disabled {
            background-color: var(--red);
            cursor: not-allowed;
        }
        
        .payment-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.7);
            z-index: 1000;
            overflow-y: auto;
        }
        
        .modal-content {
            background-color: white;
            margin: 5% auto;
            padding: 2rem;
            width: 90%;
            max-width: 600px;
            border-radius: 5px;
            position: relative;
        }
        
        .close-btn {
            position: absolute;
            top: 1rem;
            right: 1rem;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        .payment-option {
            margin: 1.5rem 0;
            padding: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        
        .payment-option h3 {
            margin-top: 0;
        }
        
        .qr-code {
            width: 200px;
            height: 200px;
            margin: 1rem auto;
            display: block;
            background-color: #f5f5f5;
            padding: 10px;
            border-radius: 5px;
        }
        
        .payment-instructions {
            background-color: var(--light-gray);
            padding: 1rem;
            border-radius: 5px;
            margin-top: 1rem;
        }
        
        footer {
            background-color: var(--gray);
            color: white;
            padding: 2rem 0;
            margin-top: 3rem;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .footer-section h3 {
            color: var(--gold);
            margin-top: 0;
        }
        
        .copyright {
            text-align: center;
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid #555;
        }
        
        .note {
            font-style: italic;
            color: #666;
            margin-top: 1rem;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .sections-container {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <img src="https://www.manutd.com/assets/images/logo.png" alt="Manchester United Logo" class="logo">
            <h1>Manchester United vs Arsenal</h1>
            <div class="match-info">
                <p>Premier League | Old Trafford | August 17, 2024 | 15:30 BST</p>
            </div>
        </div>
    </header>
    
    <main class="container">
        <h2>Stadium Seating Map & Ticket Availability</h2>
        <img src="https://www.manutd.com/assets/images/tickets/seating-plan.jpg" alt="Old Trafford Seating Plan" class="stadium-map">
        
        <p>Secure your seats for this highly anticipated Premier League clash at the Theatre of Dreams. Tickets are selling fast - don't miss your chance to witness this historic rivalry live at Old Trafford.</p>
        
        <div class="sections-container">
            <div class="section">
                <span class="section-location">North Stand - Home Side</span>
                <h3>North Stand Tier 1</h3>
                <p>Direct view of the pitch with excellent atmosphere from passionate home supporters. Located on the north side of the stadium behind one goal.</p>
                <div class="price">£220 per ticket</div>
                <button class="btn btn-get-now get-tickets-btn">Get Now</button>
            </div>
            
            <div class="section sold-out">
                <span class="section-location">Stretford End - Home Side</span>
                <h3>Stretford End Tier 2</h3>
                <p>The legendary stand with the most vocal United supporters. Located west side behind the goal. Limited availability.</p>
                <div class="price">£240 per ticket</div>
                <button class="btn btn-disabled" disabled>Sold Out</button>
            </div>
            
            <div class="section">
                <span class="section-location">East Stand - Home Side</span>
                <h3>Family Stand</h3>
                <p>Great family-friendly atmosphere with excellent pitch views. Located on the east side of the stadium.</p>
                <div class="price">£190 per ticket</div>
                <button class="btn btn-get-now get-tickets-btn">Get Now</button>
            </div>
            
            <div class="section sold-out">
                <span class="section-location">South Stand - Away Side</span>
                <h3>Away Support Section</h3>
                <p>Designated area for Arsenal supporters. Strictly no home fans. Located on the south side.</p>
                <div class="price">£210 per ticket</div>
                <button class="btn btn-disabled" disabled>Sold Out</button>
            </div>
            
            <div class="section">
                <span class="section-location">West Stand - Home Side</span>
                <h3>Premium Seating</h3>
                <p>Premium seating with excellent facilities and best views of the pitch. Located on the west side opposite the dugouts.</p>
                <div class="price">£240 per ticket</div>
                <button class="btn btn-get-now get-tickets-btn">Get Now</button>
            </div>
            
            <div class="section">
                <span class="section-location">North West Corner - Home Side</span>
                <h3>North West Quadrant</h3>
                <p>Corner section with good views of both goals and the Stretford End. Located between north and west stands.</p>
                <div class="price">£180 per ticket</div>
                <button class="btn btn-get-now get-tickets-btn">Get Now</button>
            </div>
        </div>
    </main>
    
    <!-- Payment Modal -->
    <div id="paymentModal" class="payment-modal">
        <div class="modal-content">
            <span class="close-btn">&times;</span>
            <h2>Complete Your Ticket Purchase</h2>
            <p>Minimum purchase: 2 tickets</p>
            
            <div class="payment-option">
                <h3>Option 1: Skrill Payment</h3>
                <p>Secure digital wallet payment - Fast, safe and easy</p>
                
                <div class="payment-instructions">
                    <h4>How to Pay via Skrill App:</h4>
                    <ol>
                        <li><strong>Open Skrill App</strong> on your mobile device or visit <a href="https://www.skrill.com" target="_blank">www.skrill.com</a></li>
                        <li><strong>Log in</strong> to your Skrill account</li>
                        <li>Tap <strong>"Send Money"</strong> or <strong>"Pay"</strong> option</li>
                        <li>Enter recipient details:
                            <ul>
                                <li><strong>Email:</strong> jk3054794@gmail.com</li>
                                <li><strong>Amount:</strong> [Total from your selected tickets] GBP</li>
                            </ul>
                        </li>
                        <li>In <strong>Reference/Message</strong> field, enter: <code>MUNARS[YourName]</code></li>
                        <li>Select your <strong>payment method</strong> (Skrill balance, card, or bank transfer)</li>
                        <li>Review details and confirm payment</li>
                        <li>Take screenshot of payment confirmation</li>
                    </ol>
                    
                    <div style="display: flex; justify-content: space-between; margin: 1rem 0;">
                        <div style="text-align: center;">
                            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Skrill_logo.svg/1200px-Skrill_logo.svg.png" alt="Skrill Logo" style="height: 60px; margin-bottom: 0.5rem;">
                            <p>Official Skrill Partner</p>
                        </div>
                        <div style="text-align: center;">
                            <img src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=jk3054794@gmail.com&amount=[Amount]&currency=GBP&note=MUNARS" alt="Skrill QR Payment" style="height: 150px;">
                            <p>Scan to Pay</p>
                        </div>
                    </div>
                    
                    <div style="background-color: #f0f8ff; padding: 1rem; border-radius: 5px; margin-top: 1rem;">
                        <h4>Important Notes:</h4>
                        <ul>
                            <li>Ensure you send payment in <strong>GBP (British Pounds)</strong></li>
                            <li>Include the correct reference <code>MUNARS[YourName]</code></li>
                            <li>Payments typically process within 15 minutes</li>
                            <li>Contact us immediately if payment fails</li>
                        </ul>
                    </div>
                    
                    <button class="btn btn-get-now" onclick="window.open('https://www.skrill.com/en/pay/', '_blank')" style="margin-top: 1rem; width: 100%;">
                        Pay Now via Skrill
                    </button>
                </div>
            </div>
            
            <div class="payment-option">
                <h3>Option 2: Bitcoin Payment</h3>
                <p>Secure cryptocurrency payment</p>
                
                <div class="payment-instructions">
                    <h4>Bitcoin Address (Taproot):</h4>
                    <p><code>bc1p2mlnlmluamk80a3xlw9d3luucr0crtcne8xyepl88n5k4vfznf7skd4t4r</code></p>
                    <p><strong>Amount:</strong> [BTC equivalent of your total]</p>
                    <p><strong>Network:</strong> Bitcoin (Taproot compatible)</p>
                </div>
            </div>
            
            <div class="payment-option">
                <h3>Option 3: M-Pesa via Wise</h3>
                <p>Fast and secure payment via M-Pesa</p>
                
                <div class="payment-instructions">
                    <h4>Wise Account Details:</h4>
                    <p><strong>Account Name:</strong> James Warigithi Karanja</p>
                    <p><strong>Phone Number:</strong> +254 715 869346</p>
                    <p><strong>Country:</strong> Kenya</p>
                    <p><strong>Payment Method:</strong> M-Pesa</p>
                    <p><strong>Payment Reference:</strong> MUNARS[YourName]</p>
                    
                    <div class="qr-code">
                        <!-- QR code would be generated here -->
                        <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=M-PesaPaybill%3A247247%26AccountNumber%3D715869346%26Reference%3DMUNARS" alt="M-Pesa QR Code">
                    </div>
                    
                    <p class="note">Wise details of our abroad ticket dealer</p>
                    
                    <button class="btn btn-get-now" onclick="window.open('https://wise.com/pay/me/jameswk', '_blank')">Pay via Wise Directly</button>
                </div>
            </div>
            
            <div class="payment-instructions">
                <h4>After Payment:</h4>
                <p>Please send your payment confirmation to:</p>
                <p><strong>Email:</strong> UK-TICKETS.BESTDEALS@proton.mail</p>
                <p><strong>WhatsApp:</strong> +44 7832 714017</p>
                <p>Include your name, contact details, and preferred seating section.</p>
                <p>E-tickets will be sent within 24 hours of payment confirmation.</p>
            </div>
        </div>
    </div>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>About Our Tickets</h3>
                    <p>We are an official secondary ticket partner for Manchester United FC, providing verified tickets for all home matches at Old Trafford.</p>
                </div>
                
                <div class="footer-section">
                    <h3>Refund Policy</h3>
                    <p>Refund requests must be made at least 7 days prior to match day:</p>
                    <ol>
                        <li>Email refund request to UK-TICKETS.BESTDEALS@proton.mail</li>
                        <li>Include your payment details and ticket reference</li>
                        <li>Allow 5-7 business days for processing</li>
                        <li>10% processing fee applies to all refunds</li>
                    </ol>
                </div>
                
                <div class="footer-section">
                    <h3>Contact Us</h3>
                    <p>For any inquiries or support:</p>
                    <p>Email: UK-TICKETS.BESTDEALS@proton.mail</p>
                    <p>WhatsApp: +44 7832 714017</p>
                    <p>Business Hours: 9:00-17:00 GMT, Mon-Fri</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2024 Manchester United Official Ticket Partner. This service is operated independently from Manchester United Football Club.</p>
            </div>
        </div>
    </footer>
    
    <script>
        // Show payment modal when Get Now button is clicked
        const getTicketBtns = document.querySelectorAll('.get-tickets-btn');
        const paymentModal = document.getElementById('paymentModal');
        const closeBtn = document.querySelector('.close-btn');
        
        getTicketBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                paymentModal.style.display = 'block';
                document.body.style.overflow = 'hidden';
            });
        });
        
        closeBtn.addEventListener('click', () => {
            paymentModal.style.display = 'none';
            document.body.style.overflow = 'auto';
        });
        
        window.addEventListener('click', (e) => {
            if (e.target === paymentModal) {
                paymentModal.style.display = 'none';
                document.body.style.overflow = 'auto';
            }
        });
    </script>
</body>
</html>
