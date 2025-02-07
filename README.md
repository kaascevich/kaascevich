![me! but not quite.](https://github.com/user-attachments/assets/c0ce4e2a-13b0-4154-bcf9-27324a35bcf9 "me! but not quite.")

いらっしゃいませ to my tiny little haven on the internet!

I'm Kaleb, and I'm quite content to float around aimlessly around here. open source is something I quite enjoy, though I'm not afraid to _use_ closed source software as long as it's of 🍎-level quality.

```swift
import Foundation
import PersonDescription

struct Me: Person {
  let name = Name("Kaleb A. Ascevich", pronunciation: "KAY-lub AICE-uh-vitch")
  let pronouns = ("he", "him", "his")
  let birthday: Date = DateComponents(
    calendar: .current,
    year: 2007, month: 11, day: 9
  ).date!
  let address = Address(state: .florida, country: .usa)

  var langs: [Lang] = [.swift, .rust, .nix]
  let shell = Shell.nushell

  var apps: [_: [App]] = [
    "ide": ["Xcode", "VSCodium"],
    "term": ["iTerm2"],
    "music": ["Apple Music"],
    "browser": ["Safari"],
  ]
  var devices: [_: (any Device, [OS])] = [
    "Kaleb's MacBook": (
      Mac(.macbookAir, 10, 1),
      [.macOS]
    ),
    "macbookair61": (
      Mac(.macbookAir, 6, 1),
      [.linux(distro: "Debian")]
    ),
    "zenbook": (
      PC(.laptop, "ASUS"),
      [.linux(distro: "Bazzite")]
    ),
    "imacg4": (
      Mac(.powerMac, 4, 2),
      [.macOS, .macOS]
    ),
    "Kaleb's Ally": (
      PC(.handheld, "ASUS"),
      [.linux(distro: "Bazzite")]
    ),
  ]
}

extension Me {
  var age: Int {
    Calendar.current.components(
      [.year], from: birthday, to: .now
    ).year!
  }
}
```

and, most importantly,

```swift
extension Me {
  let favoriteQuote = Quote(
    """
    The people who are crazy enough to think they can change the
    world, are the ones who do.
    """,
    by: Name("Steve Jobs")
  )
}
```

## other marginally less important details

- I want **_nothing_** to do with web development. JavaScript is just… [bad](https://www.destroyallsoftware.com/talks/wat).
- my socialization skills are… lacking. it's getting better, but they're still quite lacking. just take that into account if you want to talk to me.
- I'm not online *too* often, because school exists (which is absolutely not unfortunate in any way other than that).

## links

- [my *true* tiny home online](https://kaascevich.github.io)
- [email](mailto:cloths-fringe0s@icloud.com) (don't expect an immediate reply, though — I tend to keep my inbox tidy)
