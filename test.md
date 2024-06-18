<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Copy Text to Clipboard</title>
</head>
<body>
    <div style="display: flex; flex-direction: column; align-items: center; margin-top: 50px;">
        <textarea id="text-box" readonly style="width: 80%; height: 150px; padding: 10px; margin-bottom: 10px; font-size: 16px; border: 1px solid #ccc; border-radius: 5px; resize: none;">
This is the text that will be displayed in a box and can be copied to the clipboard.
        </textarea>
        <button id="copy-button" style="padding: 10px 20px; font-size: 16px; color: #fff; background-color: #007bff; border: none; border-radius: 5px; cursor: pointer;">Copy Text</button>
    </div>
    <script>
        document.getElementById('copy-button').addEventListener('click', function() {
            var textBox = document.getElementById('text-box');
            textBox.select();
            textBox.setSelectionRange(0, 99999); // For mobile devices
            try {
                var successful = document.execCommand('copy');
                var msg = successful ? 'successful' : 'unsuccessful';
                console.log('Copying text command was ' + msg);
            } catch (err) {
                console.log('Oops, unable to copy');
            }
            alert('Text copied to clipboard');
        });
    </script>
</body>
</html>
