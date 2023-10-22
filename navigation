# #swiftui Navigation
App’i oluşturmaya başlamadan önce React Native Developer’lar olarak öncellikle navigation yapısını kurarız. Bu yapıyı kurarken React Navigation’ı kullanarak tüm App’i bir container’a sararız. Öncelikle ben SwiftUI’da buna benzer bir yapıyla başladım ve “Neyesek” uygulamamda ise ihtiyacım bir TabNavigator’dı. Onu da ContentView dosyama şu şekilde ekledim.

```
import SwiftUI

struct ContentView: View {
    var body: some View {
       Tab()
    }
}

#Preview {
    ContentView()
}

```

Ekranlarımı da şu şekilde tanımladım. Yukarıda kullandığım “Tab” aşağıdaki dosyadan geliyor.
![](image.png)<!-- {"width":290} -->


```
import SwiftUI

struct Tab: View {
    var body: some View {
        NavigationView {
            TabView {
                DiscoveryMain()
                    .tabItem {
                        Label("Keşfet", systemImage: "house")
                    }
                SearchMain()
                    .tabItem {
                        Label("Arama", systemImage: "magnifyingglass")
                    }
                LikesMain()
                    .tabItem {
                        Label("Beğeniler", systemImage: "heart")
                    }
                HistoryMain()
                    .tabItem {
                        Label("Geçmiş", systemImage: "clock")
                    }
                GeneralMain()
                    .tabItem {
                        Label("Genel", systemImage: "gear")
                    }
            }
        }
    }
}

```

Örneğin buradaki Ekranlardan biri üzerinden gidelim. Bunun için HistoryMain’i seçiyorum. Başlangıç için bu şekilde geliyor.

```
import SwiftUI

struct HistoryMain: View {
    var body: some View {
        Text(/*@START_MENU_TOKEN@*/"Hello, World!"/*@END_MENU_TOKEN@*/)
    }
}

#Preview {
    HistoryMain()
}

```
