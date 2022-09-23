
# notes
dotnet new blazorwasm -o mddocx2 --pwa -f net6.0 
dotnet add package Open-XML-SDK --version 2.9.1
dotnet watch
dotnet publish -c Release
cd bin/Release/net6.0/publish/wwwroot
surge . mddocx2.surge.sh
