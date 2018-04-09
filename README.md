# Google Material Icons


<p>Plugin de icones para multiplataforma (iOS/Android).</p>
<p>link Google Material -> https://material.io/icons/</p>

# Plataformas Suportadas

- Xamarin.Android
- Xamarin.iOS
- Windows Phone 

# Link do Plugin 

Adicione o pacote Nuguet (https://www.nuget.org/packages/Xam.FormsPlugin.MaterialIcons) no seu projeto PCL e nos outros proejtos (Android, iOS).

**Adicionando na XAML (PCL)**

```
xmlns:mi="clr-namespace:MaterialIcons.FormsPlugin.Abstractions;assembly=MaterialIcons.FormsPlugin.Abstractions"
```

Chamando o icone
```
<mi:IconLabel 
  Icon="ic_android" 
  FontSize="48" 
  TextColor="Blue"/>
 ```

**Android**
- Insira no arquivo MainActivity.cs
```
Xamarin.Forms.Init(this, savedInstanceState);  
MaterialIconControls.Init();
```

**iOS**
- Insira no arquivo AppDelegate.cs
```
Xamarin.Forms.Init();  
MaterialIconControls.Init();
```
- **Atenção:** Inclua no arquivo **info.plist**
```
<key>UIAppFonts</key>
<array>
    <string>MaterialIcons-Regular.ttf</string>
</array>
```

# Referência Original:
- https://github.com/jsmarcus/Xamarin.Plugins/tree/master/MaterialIcons
