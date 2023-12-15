```swift
import SwiftUI

struct ContentView: View {
    @State private var backgroundColor: Color = .black
    
    var body: some View {
        VStack {
            Text("Change Background Color")
                .padding()
            
            Button("Red") {
                //버튼 실행했을 때 액션
                backgroundColor = .red
            }
            .background(Color.red) // 원하는 색상으로 변경
            .padding()
            
            Button("Blue") {
                backgroundColor = .blue
            }
            .background(Color.blue)
            .padding()
        }
        .frame(maxWidth: .infinity, maxHeight: .infinity)
        .background(backgroundColor)
    }
}
#Preview {
    ContentView()
}

```
