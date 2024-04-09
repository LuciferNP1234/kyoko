<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Waifu Generator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            background-color: hsla(0, 100%, 50%, 1);
            background-image: radial-gradient(at 40% 20%, hsla(28, 100%, 74%, 1) 0px, transparent 50%),
                radial-gradient(at 80% 0%, hsla(189, 100%, 56%, 1) 0px, transparent 50%),
                radial-gradient(at 0% 50%, hsla(355, 100%, 93%, 1) 0px, transparent 50%),
                radial-gradient(at 80% 50%, hsla(340, 100%, 76%, 1) 0px, transparent 50%),
                radial-gradient(at 0% 100%, hsla(22, 100%, 77%, 1) 0px, transparent 50%),
                radial-gradient(at 80% 100%, hsla(242, 100%, 70%, 1) 0px, transparent 50%),
                radial-gradient(at 0% 0%, hsla(343, 100%, 76%, 1) 0px, transparent 50%);
        }
 * {
            margin: 0;
            padding: 0;
            outline: none;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }
    </style>
</head>

<body>
    <div class="container">
        <a href="https://api.rei.my.id" class="btn btn-primary my-3">HOME</a>
        <h1 class="text-center mb-4">Waifu Generator</h1>
        <p class="lead text-center">Generate a huge variety of waifu images for you!</p>

 <div class="text-center my-4">
            <img src="https://img.shields.io/badge/SCHEME-HTTPS-a3be8c?style=flat-square" alt="Scheme"
                class="me-2">
            <img src="https://img.shields.io/badge/AUTHENTICATION-NONE-ebcb8b?style=flat-square" alt="Authentication"
                class="me-2">
            <img src="https://img.shields.io/badge/LIMITATION-50%20200%20OK%20%2F%201min-88C0D0?style=flat-square"
                alt="Limitation">
        </div>

 <h2 class="text-center mb-3">Categories</h2>
        <div class="row justify-content-center">
            <div class="col-md-6">
                <table class="table table-striped">
                    <thead>
                        <tr>
                            <th>SFW</th>
                            <th>NSFW</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>waifu</td>
                            <td>waifu</td>
                        </tr>
                        <tr>
                            <td>neko</td>
                            <td>trap</td>
                        </tr>
                        <!-- Add more categories as needed -->
                    </tbody>
                </table>
            </div>
        </div>

  <h2 class="text-center mb-3">Get image</h2>
        <div class="row justify-content-center">
            <div class="col-md-6">
                <table class="table">
                    <thead>
                        <tr>
                            <th>URL</th>
                            <th>Request Type</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>https://waifu.rei.my.id/{type}/{category}</td>
                            <td>GET</td>
                        </tr>
                        <tr>
                            <td>https://waifu.rei.my.id/many/{type}/{category}</td>
                            <td>GET</td>
                        </tr>
                    </tbody>
                </table>
                <p class="text-muted">Valid types are sfw and nsfw.</p>
            </div>
        </div>

 <h3 class="text-center mt-4">Example</h3>
        <div class="row justify-content-center">
            <div class="col-md-6">
                <h4>Request</h4>
                <pre><code class="language-shell">curl https://waifu.rei.my.id/nsfw/trap</code></pre>
                <h4>Response</h4>
                <pre><code class="language-json">{
    "RequestTimestamp":1709703055,
    "RequestStatus":"success",
    "RequestCode":200,
    "RequestResult":{
        "url":"https://i.rei.my.id/QvOUXvM.jpg"
    }
}</code></pre>
            </div>
        </div>
    </div>
</body>

</html>
