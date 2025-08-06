<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JPEG to PDF Converter</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 15px; background: #f0f2f5; }
        .container { background: white; padding: 20px; border-radius: 10px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        h1 { color: #2c3e50; text-align: center; }
        #uploadBtn { display: block; width: 100%; padding: 15px; background: #3498db; color: white; border: none; border-radius: 5px; font-size: 16px; margin: 20px 0; text-align: center; }
        #preview { margin-top: 20px; text-align: center; }
        #previewImg { max-width: 100%; max-height: 200px; display: none; margin: 0 auto; }
        #convertBtn { width: 100%; padding: 15px; background: #2ecc71; color: white; border: none; border-radius: 5px; font-size: 16px; margin-top: 20px; display: none; }
        #status { margin: 10px 0; padding: 10px; border-radius: 5px; display: none; }
        .success { background: #d4edda; color: #155724; }
        .error { background: #f8d7da; color: #721c24; }
    </style>
</head>
<body>
    <div class="container">
        <h1>JPEG to PDF Converter</h1>
        <input type="file" id="fileInput" accept="image/jpeg" style="display: none;">
        <button id="uploadBtn">Select Photo</button>
        <div id="preview"><img id="previewImg" alt="Preview"></div>
        <button id="convertBtn">Create PDF</button>
        <div id="status"></div>
    </div>

    <script>
        // DOM Elements
        const fileInput = document.getElementById('fileInput');
        const uploadBtn = document.getElementById('uploadBtn');
        const previewImg = document.getElementById('previewImg');
        const convertBtn = document.getElementById('convertBtn');
        const statusDiv = document.getElementById('status');
        
        // File Input Click
        uploadBtn.addEventListener('click', () => fileInput.click());
        
        // File Selected
        fileInput.addEventListener('change', function(e) {
            if(e.target.files.length > 0) {
                const reader = new FileReader();
                reader.onload = function(event) {
                    previewImg.src = event.target.result;
                    previewImg.style.display = 'block';
                    convertBtn.style.display = 'block';
                    showStatus('Image selected', 'success');
                };
                reader.readAsDataURL(e.target.files[0]);
            }
        });
        
        // Convert to PDF
        convertBtn.addEventListener('click', function() {
            if(!fileInput.files[0]) {
                showStatus('Please select an image first', 'error');
                return;
            }
            
            convertBtn.disabled = true;
            convertBtn.textContent = 'Creating PDF...';
            
            // Simple PDF Creation
            const { jsPDF } = window.jspdf;
            const pdf = new jsPDF();
            pdf.addImage(previewImg.src, 'JPEG', 15, 15, 180, 0);
            pdf.save('converted.pdf');
            
            convertBtn.disabled = false;
            convertBtn.textContent = 'Create PDF';
            showStatus('PDF downloaded!', 'success');
        });
        
        // Show Status Message
        function showStatus(message, type) {
            statusDiv.textContent = message;
            statusDiv.className = type;
            statusDiv.style.display = 'block';
        }
    </script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
</body>
</html>