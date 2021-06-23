# Update Content in Real-time using SignalR

<h2>About</h2>
<p>Server-side code push content to connected clients in real-time using SignalR.</p>

<h2>Tools</h2>
<ul>
    <li>.NET 5.0+</li>
    <li>VS Code</li>
</ul>

<h2>How to Run</h2>
<ol>
    <li>Run <code>dotnet restore</code></li>
    <li>Change the ConnectionString in appsettings.json</li>
    <li>Run <code>dotnet ef migrations add {migration name}</code></li>
    <li>Run <code>dotnet ef database update</code></li>
    <li>Run <code>dotnet run</code></li>
</ol>
