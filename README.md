💻 Flip Card Website — Chandu Software Solutions
🌟 Overview
This project is a 3D flip card web component that showcases your company, Chandu Software Solutions.

The front side features a video background.

On hover, it flips to reveal a detailed company description and a "Register" button that links to your form.

🚀 Features
✅ Smooth 3D flip animation on hover

✅ Video background on front

✅ Attractive gradient animated background on the back

✅ Responsive "Register" button with gradient effect

✅ Full-page attractive background image

🗂️ File Structure
index.html
style.css
README.md (this file)

🧩 How it works
✨ HTML Structure
.card_container: Main wrapper that provides perspective for 3D effect.

.card: Inner container that holds both front and back sides and is responsible for the flip animation.

.frontcard: Shows a looping video.

.backcard: Contains company description and a button linking to a registration form.

💅 CSS Key Points
📌 Container & Flip

.card_container {
  perspective: 1000px;
}
.card {
  transform-style: preserve-3d;
  transition: transform 0.6s ease-in-out;
}
.card_container:hover .card {
  transform: rotateY(180deg);
}

perspective gives depth.

transform-style: preserve-3d maintains child 3D positioning.

hover triggers rotateY(180deg) for flipping.

🎥 Front Card
.frontcard video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

The video fills the card and loops seamlessly.

🌈 Back Card
.backcard {
  background: linear-gradient(90deg, #833ab4, #fd1d1d, #fcb045, #833ab4);
  background-size: 300% 300%;
  transform: rotateY(180deg);
  animation: flow-border 3s linear infinite;
}

Beautiful animated gradient background.

Note: You must define @keyframes flow-border if not already included.

Example keyframes for background movement

@keyframes flow-border {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

📝 Back Card Content

.backcard_content {
  background-color: black;
  color: white;
  padding: 16px;
  border-radius: 13px;
  overflow-y: auto;
}
.name {
  color: #00ffff;
}
.description {
  color: #f0e68c;
}

Dark theme with bright text colors for readability.

🔘 Button
.btn{
  background: linear-gradient(135deg, #00ffcc, #3366ff);
  color: white;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
  transition: background 0.3s ease;
}
.btn:hover {
  background: linear-gradient(135deg, #ff0066, #6600ff);
}

Gradient background, rounded corners, and smooth hover transitions.

🌄 Page Background
body {
  background-image: url("https://t3.ftcdn.net/jpg/02/98/90/74/360_F_298907406_MPWwwLXkNGDQjbX69PpYuE1i2EZntqs6.jpg");
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

Full-screen attractive background image.

⚙️ Usage
1️⃣ Replace your video file source if needed (currently Pink & Blue Futuristic Gaming Channel Youtube Intro.mp4).
2️⃣ Customize text and description to match your company.
3️⃣ Update the button link to your registration form if different.
4️⃣ Add @keyframes flow-border animation if missing.

💡 Future Improvements
Add responsive adjustments for mobile devices.

Add multiple cards if showcasing multiple services.

Add smooth transitions for additional inner content.

💬 Contact
For any clarifications or help, feel free to contact:
Email: chanduinternship@gmail.com
Mobile: 8008348678

