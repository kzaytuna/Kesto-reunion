# Kesto-reunion
Keato Reunion Flyer
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2025 Annual Kesto Reunion Flyer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #e0ffe0; /* A very light, fresh green */
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            padding: 1rem;
        }
        .flyer-container {
            background: linear-gradient(135deg, #f0fff4 0%, #d4edda 100%); /* Soft, inviting green gradient */
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2); /* More pronounced shadow */
            border-radius: 30px; /* More rounded corners */
            overflow: hidden;
            border: 3px solid #38a169; /* A vibrant green border */
            max-width: 600px; /* Slightly wider for better presentation */
            width: 100%;
            animation: fadeIn 1s ease-out; /* Simple fade-in animation */
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .header-bg {
            background-color: #2f855a; /* Deep emerald green */
            color: white;
            position: relative;
            overflow: hidden;
            padding: 2.5rem 1.5rem; /* More padding for header */
            border-bottom: 5px solid #38a169; /* Accent line */
        }
        .header-bg::before, .header-bg::after {
            content: '';
            position: absolute;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            opacity: 0.8;
            filter: blur(10px);
        }
        .header-bg::before {
            width: 120px; height: 120px;
            top: -30px; left: -30px;
        }
        .header-bg::after {
            width: 100px; height: 100px;
            bottom: -20px; right: -20px;
        }
        .header-title {
            font-size: 2.8rem; /* Larger title */
            line-height: 1.1;
            font-weight: 900; /* Extra bold */
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
            margin-bottom: 0.5rem;
        }
        @media (min-width: 640px) {
            .header-title {
                font-size: 3.5rem;
            }
        }

        .detail-card {
            background-color: #ffffff; /* Pure white for crispness */
            border-left: 8px solid #48bb78; /* Brighter green accent */
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.08); /* Softer shadow */
            padding: 1.5rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .detail-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.12);
        }
        .detail-heading {
            font-size: 1.8rem;
            font-weight: 800;
            color: #2f855a; /* Deep emerald for headings */
            margin-bottom: 0.75rem;
        }
        .detail-text {
            font-size: 1.15rem;
            color: #333;
            line-height: 1.6;
        }
        .map-embed {
            border-radius: 15px;
            overflow: hidden;
            border: 2px solid #48bb78;
            margin-top: 1rem;
        }
        .map-link {
            color: #38a169; /* Vibrant green for link */
            text-decoration: underline;
            font-weight: 700;
            transition: color 0.2s ease;
        }
        .map-link:hover {
            color: #2f855a; /* Darker green on hover */
        }
        .list-disc-custom {
            list-style-type: none; /* Remove default bullet */
            padding-left: 1.5rem;
        }
        .list-disc-custom li::before {
            content: '•'; /* Custom bullet point */
            color: #48bb78; /* Green bullet */
            display: inline-block;
            width: 1em;
            margin-left: -1.5em;
        }
        .calendar-button {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 0.75rem 1.5rem; /* More padding for a bolder button */
            border-radius: 9999px; /* Pill shape */
            font-weight: 700;
            margin-top: 1rem; /* Space from content above */
            background-color: #38a169; /* Primary green for the button */
            color: white;
            transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Stronger shadow */
            text-decoration: none; /* Remove underline for links */
            font-size: 1.1rem; /* Slightly larger text */
        }
        .calendar-button:hover {
            background-color: #2f855a; /* Darker green on hover */
            transform: translateY(-3px); /* More pronounced lift */
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.25);
        }
    </style>
</head>
<body>
    <div class="flyer-container">
        <!-- Header Section -->
        <div class="header-bg text-center rounded-t-[28px]">
            <h1 class="header-title">
                2025 Annual Kesto Reunion
            </h1>
        </div>

        <!-- Event Details Section -->
        <div class="p-6 sm:p-8 md:p-10 space-y-8">
            <div class="detail-card">
                <h2 class="detail-heading">🗓️ Date & Time</h2>
                <p class="detail-text">
                    <span class="font-extrabold text-green-800">July 13, 2025</span><br>
                    <span class="font-semibold">11:00 AM - 9:00 PM</span>
                </p>
            </div>

            <div class="detail-card">
                <h2 class="detail-heading">📍 Location</h2>
                <p class="detail-text font-semibold mb-4">
                    Stony Creek Metropark<br>
                    Mount Vernon Picnic Shelter
                </p>
                <div class="map-embed w-full">
                    <!-- Embedded Google Map with Pin -->
                    <iframe
                        src="https://maps.google.com/maps?q=42.731418,-83.095446&hl=en&z=14&output=embed"
                        width="100%"
                        height="300"
                        style="border:0;"
                        allowfullscreen=""
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
                <p class="mt-4 text-center">
                    <a href="https://maps.apple.com/place?address=Stony%20Creek%20Metropark,%20Mt%20Vernon%20Dr,%20Washington,%20MI%20%2048094,%20United%20States&coordinate=42.731418,-83.095446&name=Stony%20Creek%20Metropark&map=h" target="_blank" class="map-link">
                        Click here for Map
                    </a>
                </p>
            </div>

            <div class="detail-card">
                <h2 class="detail-heading">🏊 What to Bring</h2>
                <p class="detail-text">
                    Don't forget your <span class="font-extrabold text-green-800">Swim Attire</span> and <span class="font-extrabold text-green-800">Towels</span> for some refreshing water fun!
                </p>
            </div>

            <div class="detail-card text-left">
                <h2 class="detail-heading">🚗 Directions from Metro Detroit Area</h2>
                <p class="detail-text mb-3">
                    Stony Creek Metropark is located north of Rochester Hills, accessible from M-53 (Van Dyke Freeway) or M-59 (Hall Road).
                </p>
                <ul class="list-disc-custom space-y-2">
                    <li><strong class="text-green-700">From M-53 (Van Dyke Freeway):</strong> Take M-53 North to the 26 Mile Road exit. Turn left (west) onto 26 Mile Road. The park entrance will be on your right.</li>
                    <li><strong class="text-green-700">From M-59 (Hall Road):</strong> Head east or west on M-59 until you reach M-53 (Van Dyke Freeway). Go north on M-53 and follow the directions above.</li>
                    <li><strong class="text-green-700">Inside the Park:</strong> Once inside, follow signs for "Mount Vernon Picnic Shelter."</li>
                </ul>
            </div>

            <div class="detail-card text-center">
                <h2 class="detail-heading">➕ Add to Calendar</h2>
                <button id="add-to-calendar-button" class="calendar-button">
                    <svg class="w-6 h-6 mr-2" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
                    Add Event to Calendar
                </button>
            </div>
        </div>

        <!-- Footer Section -->
        <div class="bg-gray-800 text-white py-6 rounded-b-[28px] text-center">
            <p class="text-lg font-medium">
                We can't wait to celebrate with you! See you there!
            </p>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const eventTitle = "2025 Annual Kesto Reunion";
            const eventLocationText = "Stony Creek Metropark, Mount Vernon Picnic Shelter";
            const eventDescription = "2025 Annual Kesto Reunion. Bring Swim Attire and towels.";
            const eventGeo = "42.731418,-83.095446"; // Exact coordinates

            // Event times in EDT (Eastern Daylight Time, UTC-4)
            // 11:00 AM EDT on July 13, 2025 = 15:00 UTC on July 13, 2025
            // 9:00 PM EDT on July 13, 2025 = 01:00 UTC on July 14, 2025 (next day)
            const icsStartUTC = "20250713T150000Z";
            const icsEndUTC = "20250714T010000Z";

            document.getElementById('add-to-calendar-button').addEventListener('click', function() {
                const now = new Date();
                const dtStamp = now.toISOString().replace(/[-:]|\.\d{3}/g, '') + 'Z';
                const uid = Date.now().toString() + "@kestoreunion.com"; // More unique ID

                const icsContent = `BEGIN:VCALENDAR
VERSION:2.0
PRODID:-//Kesto Reunion//EN
BEGIN:VEVENT
UID:${uid}
DTSTAMP:${dtStamp}
DTSTART:${icsStartUTC}
DTEND:${icsEndUTC}
SUMMARY:${eventTitle}
LOCATION:${eventLocationText}
GEO:${eventGeo}
DESCRIPTION:${eventDescription}
END:VEVENT
END:VCALENDAR`;

                const blob = new Blob([icsContent], { type: 'text/calendar;charset=utf-8' });
                const url = URL.createObjectURL(blob);
                const a = document.createElement('a');
                a.href = url;
                a.download = 'Kesto_Reunion_2025.ics';
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                URL.revokeObjectURL(url);
            });
        });
    </script>
</body>
</html>
