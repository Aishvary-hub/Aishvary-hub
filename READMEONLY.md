Its about the music website created and hosted on w3space thank you and enjoy happy listurning........................ Name-Aishvary Gadge reg no-22071035 branch-ETC roll no-45 website link-https://neonmusicplayer.w3spaces.com webside code--

<title>Neon Band</title> <style> * { box-sizing: border-box; }
    /* Style the body */
    body {
        font-family: Arial, Helvetica, sans-serif;
        margin: 0;
        background-color: #222;
        color: white;
    }

    /* Header/logo Title */
    .header {
        padding: 50px;
        text-align: center;
        background: linear-gradient(to right, #1abc9c, #16a085);
        color: white;
    }

    /* Increase the font size of the heading */
    .header h1 {
        font-size: 50px;
        text-transform: uppercase;
    }

    /* Style the top navigation bar */
    .navbar {
        overflow: hidden;
        background-color: #333;
    }

    /* Style the navigation bar links */
    .navbar a {
        float: left;
        display: block;
        color: white;
        text-align: center;
        padding: 14px 20px;
        text-decoration: none;
        font-size: 18px;
    }

    /* Change color on hover */
    .navbar a:hover {
        background-color: #ddd;
        color: black;
    }

    /* Section styles */
    section {
        padding: 40px;
        background: rgba(31, 31, 31, 0.9);
        margin: 20px;
        border-radius: 10px;
        box-shadow: 0 6px 20px rgba(0, 0, 0, 0.7);
    }

    section h2 {
        color: #00e676;
        text-transform: uppercase;
        text-align: center;
        margin-bottom: 20px;
    }

    /* Music Player container */
    .player-container {
        background: rgba(31, 31, 31, 0.9);
        padding: 30px;
        border-radius: 20px;
        box-shadow: 0 6px 20px rgba(0, 0, 0, 0.7);
        text-align: center;
        margin: 50px auto;
        width: 100%;
        max-width: 500px;
    }

    .player-container h1 {
        font-size: 30px;
        margin-bottom: 20px;
        color: #00e676;
        text-transform: uppercase;
    }

    /* Images */
    .image-gallery {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        margin: 20px 0;
    }

    .image-gallery img {
        width: 200px; /* Adjust size as needed */
        border-radius: 10px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    }

    /* Footer */
    .footer {
        padding: 20px;
        text-align: center;
        background: linear-gradient(to right, #1abc9c, #16a085);
        color: white;
        position: fixed;
        bottom: 0;
        width: 100%;
    }

    /* Contact Us Section */
    #contact {
        padding: 60px; /* Increased padding for visibility */
    }

    #contact-form input, #contact-form textarea {
        width: 100%;
        padding: 10px;
        margin: 10px 0;
        border: 1px solid #ccc;
        border-radius: 5px;
    }

    #contact-form input[type="submit"] {
        background-color: #1abc9c;
        color: white;
        border: none;
        cursor: pointer;
    }

    #contact-form input[type="submit"]:hover {
        background-color: #16a085;
    }
</style>
Neon Band
Relax, enjoy, and listen to our music.

Home Meet the Band Playlist Contact Us
Welcome to Neon Band
Neon Band is a vibrant and energetic group of 21-year-old musicians who bring their unique sound and passion for music to life. Founded with the mission to create music that resonates with people from all walks of life, our band combines elements of pop, rock, and indie to produce catchy melodies and heartfelt lyrics. Our journey began in high school, where we discovered our love for performing together. Since then, we have been dedicated to perfecting our craft, writing original songs, and connecting with our audience.

We believe in the power of music to inspire, uplift, and bring people together. Our music is a reflection of our experiences, dreams, and the world around us. Each song we create tells a story, inviting listeners to join us on a journey of emotion and connection. Whether it's an upbeat anthem that gets you dancing or a soulful ballad that touches your heart, we aim to leave a lasting impression through our sound.

As a band, we thrive on collaboration and creativity. Our diverse backgrounds and influences shape our music, making each performance a unique experience. We're not just musicians; we're friends who share a common goal: to spread joy and positivity through our art. We invite you to explore our music, join us at our shows, and become part of the Neon Band family.

Meet the Band
Get to know the members of Neon Band! Our talented lineup includes:

Alex - Lead Vocals & Guitar: The heart and soul of our band, Alex brings raw emotion to every performance.
Jamie - Drums: With a passion for rhythm, Jamie keeps the beat and drives our songs forward.
Sam - Bass Guitar: The groove master, Sam adds depth and funk to our sound.
Taylor - Keyboards: A musical wizard, Taylor creates the rich textures that define our unique style.
Playlist
Now Playing
Select a song to play

    <div class="controls">
        <button id="prev-btn">⏮️</button>
        <button id="play-btn">▶️</button>
        <button id="next-btn">⏭️</button>
    </div>

    <div class="progress-container" id="progress-container">
        <div class="progress" id="progress"></div>
    </div>

    <div class="time-display">
        <span id="current-time">0:00</span>
        <span id="song-duration">0:00</span>
    </div>

    <!-- Volume Control -->
    <div class="volume-container">
        <label for="volume">Volume:</label>
        <input type="range" id="volume" class="volume-slider" min="0" max="1" step="0.01" value="1">
    </div>
</div>
Music Inspirations
Musical Instruments 1 Musical Instruments 2 Musical Instruments 3 Musical Instruments 4 Musical Instruments 5 Musical Instruments 6
Contact Us
<textarea rows="5" placeholder="Your Message" required></textarea>
© 2024 Neon Band. All rights reserved.

<script> const songs = [ { title: "Song 1", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" }, { title: "Song 2", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3" }, { title: "Song 3", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-3.mp3" } ]; let currentSongIndex = 0; const audio = new Audio(songs[currentSongIndex].src); const playButton = document.getElementById('play-btn'); const prevButton = document.getElementById('prev-btn'); const nextButton = document.getElementById('next-btn'); const songTitle = document.getElementById('song-title'); const currentTimeDisplay = document.getElementById('current-time'); const songDurationDisplay = document.getElementById('song-duration'); const volumeSlider = document.getElementById('volume'); const progressContainer = document.getElementById('progress-container'); const progress = document.getElementById('progress'); function loadSong(index) { audio.src = songs[index].src; songTitle.textContent = songs[index].title; audio.load(); } function playSong() { audio.play(); playButton.textContent = "⏸️"; // Change play button to pause } function pauseSong() { audio.pause(); playButton.textContent = "▶️"; // Change pause button back to play } playButton.addEventListener('click', () => { if (audio.paused) { playSong(); } else { pauseSong(); } }); prevButton.addEventListener('click', () => { currentSongIndex = (currentSongIndex - 1 + songs.length) % songs.length; loadSong(currentSongIndex); playSong(); }); nextButton.addEventListener('click', () => { currentSongIndex = (currentSongIndex + 1) % songs.length; loadSong(currentSongIndex); playSong(); }); audio.addEventListener('loadedmetadata', () => { songDurationDisplay.textContent = formatTime(audio.duration); progress.style.width = '0%'; }); audio.addEventListener('timeupdate', () => { const currentTime = audio.currentTime; currentTimeDisplay.textContent = formatTime(currentTime); progress.style.width = (currentTime / audio.duration) * 100 + '%'; }); volumeSlider.addEventListener('input', (e) => { audio.volume = e.target.value; }); function formatTime(seconds) { const minutes = Math.floor(seconds / 60); const secs = Math.floor(seconds % 60); return `${minutes}:${secs < 10 ? '0' : ''}${secs}`; } // Initialize the player with the first song loadSong(currentSongIndex); </script>
*issues-due to some technical issues to img saving services the img might not be visible
