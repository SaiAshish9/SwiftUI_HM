```
import SwiftUI
extension AnyTransition {
  static var trailingBottom: AnyTransition {
    AnyTransition.asymmetric(
      insertion: .identity,
      removal: AnyTransition.move(edge: .trailing).combined(with: .move(edge: .bottom)))
  } 
  static var leadingBottom: AnyTransition {
    AnyTransition.asymmetric(
      insertion: .identity,
      removal: AnyTransition.move(edge: .leading).combined(with: .move(edge: .bottom)))
  }
}
```

```
import SwiftUI
struct SymbolModifier: ViewModifier {
  func body(content: Content) -> some View {
    content
      .foregroundColor(Color.white)
      .font(.system(size: 128))
      .shadow(color: Color(UIColor(red: 0, green: 0, blue: 0, alpha: 0.2)), radius: 12, x: 0, y: 0)
  }
}
```

```
  // MARK: - PROPERTIES
  @Binding var showGuideView: Bool
  @Binding var showInfoView: Bool
  let haptics = UINotificationFeedbackGenerator()
  playSound(sound: "sound-click", type: "mp3")
    self.haptics.notificationOccurred(.success)
    self.showGuideView.toggle()
```

```
Capsule()
  .frame(width: 120, height: 6)
  .foregroundColor(Color.secondary)
  .opacity(0.2)
```
