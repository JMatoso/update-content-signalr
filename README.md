# Update Content in Real-time using SignalR

<h2>About</h2>
<p>
    Server-side code push content to connected clients in real-time using 
    <a href="https://dotnet.microsoft.com/apps/aspnet/signalr" target="_blank">SignalR</a>.
</p>

<h4>SignalR</h4>
<p>
    <a href="https://dotnet.microsoft.com/apps/aspnet/signalr" target="_blank">SignalR</a> is a free and open-source software 
    library for Microsoft ASP.NET that allows server code to send asynchronous notifications to client-side web applications. 
    The library includes server-side and client-side JavaScript components.
</p>
<p>
    Like the rest of ASP.NET, <a href="https://dotnet.microsoft.com/apps/aspnet/signalr" target="_blank">SignalR</a> was built 
    for high performance and is one of the fastest real-time frameworks around.
    Scale out across servers with built-in support for using <a href="https://redis.io/" target="_blank">Redis</a>, SQL Server, or Azure Service Bus 
    to coordinate messages between each instance.
</p>

<h4>Redis</h4>
<p>
    <a href="https://redis.io/" target="_blank">Redis</a> is an open source (BSD licensed), in-memory data structure store, used as a database, 
    cache, and message broker. 
    <a href="https://redis.io/" target="_blank">Redis</a> provides data structures such as strings, hashes, lists, sets, sorted sets with 
    range queries, bitmaps, hyperloglogs, geospatial indexes, and streams.
</p>

<h4>Docker Hub</h4>
<p>
    <a href="https://www.docker.com/" target="_blank">Docker</a> is a set of platform-as-a-service products that use operating system-level 
    virtualization to deliver software in packages called containers.
    Containers are granted to others and group their own software, libraries and configuration files.
</p>

<h2>Tools</h2>
<ul>
    <li>.NET 5.0+</li>
    <li>VS Code</li>
    <li><a href="https://www.docker.com/" target="_blank">Docker</a> (Optional)</li>
    <li><a href="https://redis.io/">Redis</a></li>
</ul>

<h2>How to Run</h2>
<ol>
    <li>Run <code>dotnet restore</code></li>
    <li>Change the ConnectionString in appsettings.json</li>
    <li>Run <code>dotnet ef migrations add {migration name}</code></li>
    <li>Run <code>dotnet ef database update</code></li>
    <li>Run <code>Redis</code> (if you're not using docker)</li>
    <li>Run <code>dotnet run</code></li>
    <li>Install <a href="https://hub.docker.com/_/redis" target="_blank">Redis Docker image</a> typing <code>docker pull redis</code> (if you are using Docker)</li>
    <li>Run Redis container typing <code>docker run --name some-redis -d redis redis-server --appendonly yes</code></li>
</ol>
