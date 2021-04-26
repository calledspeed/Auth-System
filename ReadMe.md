## 🔑 Authentication System

Check Out The Tutorial Below For Setting Up And Using The Auth System Note That Pastebin 
Has A Limit Of 20 Users Per Paste So Errors May Occure Would Have Used Hastebin But Its Broken

## 📒 Setup

1. Download The Class Library From Build/AuthSystem.dll
2. Add As A Reference To Your Project
3. Make A Variable 
```csharp
AuthSystem.Auth AuthSys = new AuthSystem.Auth();
```

4. Enter Your Pastebin Developer Key 
```csharp
AuthSys.DeveloperKey = "Dev Key Here";
AuthSys.LinkvertiseID = "Linkvertise ID Here";

/*
For The Linkvertise ID Enable Full Script API 
And Get The Numbers In The Script After <Script>Linkvertise(Numbers, )
Those Numbers Are Your Linkvertise ID
*/

// Put DeveloperKey And Linkvertise ID Under A Loaded Event
```

5. Make A GetKey Button
```csharp
public void GetKey_Click(object sender, EventArgs e)
{
    // Example For File Path ("Bin/Key.txt")
    AuthSys.GenerateKeyFile("File Path");
    AuthSys.PasteKey();
    AuthSys.GenKeyLink();
    AuthSys.WriteKeyFile("File Path");
}
```

6. Make Login Button
```csharp
public void Login_Click(object sender, EventArgs e)
{
    if (TextBoxName.Text == File.ReadAllText("Key File Path") { // Correct Key }
    else { // Incorrect Key }
}
```
