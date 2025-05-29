# Local Twitch Chat Viewer

A single HTML file application that allows you to view Twitch chat from any channel with various customization options. This project is designed to be simple to use by just opening the `index.html` file in your web browser.

## Features

*   **Connect to Any Twitch Channel:** Enter the username of the Twitch channel you want to view.
*   **User-configurable Credentials:**
    *   Provide your own Twitch OAuth token for connection (prefixed with `oauth:`).
    *   Set a custom nickname to use in chat.
    *   Defaults are provided for anonymous read-only access if no credentials are entered.
*   **Multiple Chat Display Styles:** Choose from several built-in themes for chat messages:
    *   **Bubble:** Rounded, semi-transparent messages with blur effect.
    *   **Vivid:** Colorful messages with gradient backgrounds and border highlights.
    *   **Light:** A clean, grayscale theme with a light background.
    *   **Pastel:** Soft, pastel-colored messages.
    *   **Twitch:** A style that mimics the default Twitch chat appearance.
    *   **PNM :** A high-contrast, vibrant style.
*   **Style Customization:**
    *   **General Controls:** Adjust common layout properties for *all* message styles using sliders for:
        *   Max Message Width
        *   Vertical & Horizontal Padding
        *   Corner Radius
        *   Message Spacing
    *   **Vivid Style Specifics:** The "Vivid" style has additional unique controls for Shadow Intensity and Border Width.
*   **Toggleable Timestamps:** Show or hide timestamps for each message.
*   **Scroll Direction:** Switch between different chat display modes:
    *   **Vertical Scroll:** Standard top-to-bottom chat flow.
    *   **Horizontal Scroll:** Messages flow horizontally.
    *   **Nico Scroll:** Messages fly across the screen from right to left, reminiscent of Nico Nico Douga.
*   **Nico Scroll Speed Control:** When "Nico Scroll" is active, a slider appears to control the animation duration (speed) of the flying messages.
*   **Chat Scale Control:** Adjust the overall size of the chat display area using a slider, scaling from 50% to 150% of its original size. This affects all content within the chat view.
*   **Chat Management:**
    *   **Clear Chat:** Remove all current messages from the display.
    *   **Toggle Controls:** Show or hide the main controls panel using a 🎛️ icon button to maximize chat visibility.
*   **Dynamic Username Colors:** Usernames are automatically assigned distinct colors for better readability.
*   **Auto-Connect (Optional):** The application can be easily modified to auto-connect to a default channel on load (currently defaults to 'nstgaming_').

## How to Use

1.  **Download `index.html`:** Get the `index.html` file from this repository.
2.  **Obtain a Twitch OAuth Token (Recommended):**
    *   For a more stable connection and to use your own identity (even for just reading), it's recommended to use an OAuth token.
    *   You can generate one from websites like [TwitchTokenGenerator.com](https://twitchtokengenerator.com).
    *   When generating, the `chat:read` scope is sufficient for viewing chat.
    *   The token should look something like `oauth:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`.
3.  **Open in Browser:** Open the `index.html` file in your preferred web browser (e.g., Chrome, Firefox, Edge).
4.  **Configure and Connect:**
    *   Enter the **Channel Name** you want to view.
    *   (Optional) Enter your **OAuth Token**.
    *   (Optional) Enter your desired **Nickname**.
    *   Click **Connect**.
5.  **Customize:** Use the various controls to change styles, toggle timestamps, and adjust the layout to your liking.

## Structure

All the necessary HTML, CSS, and JavaScript are contained within the single `index.html` file. There are no external dependencies.
