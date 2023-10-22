# Navigation for SwiftUI

As React Native Developers, we usually start building the app by first setting up the navigation structure. In doing this, we wrap the entire app in a container using React Navigation. Similarly, I began with a structure akin to this in SwiftUI, and for my “Neyesek” app, I needed a TabNavigator. I added it to my ContentView file in the following manner:

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

I also defined my screens as shown below. The "Tab" used above is derived from the file below.

<img width="226" alt="image" src="https://github.com/oguzydz/swiftui-for-RN-developers/assets/36233491/02165da1-ebbe-4b64-8248-f2a4eb33332a">

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

For example, let’s go over one of the screens here. I’m choosing HistoryMain for this. It initially appears like this:

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
