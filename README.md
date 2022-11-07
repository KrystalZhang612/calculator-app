# KrystalZhang-Calculator App
A simple and handy calculator application developed using Swift.
## ***[Copyright and Commercial Use Disclaimer](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/README.md#please-carefully-read-licensemd-about-the-open-source-restrictions-and-the-personal-use-policy-of-this-project-under-gpl-30-license-any-commericial-uses-on-this-project-by-other-than-the-owner-krystalzhang612-or-the-authorized-users-and-organizations-including-unauthorized-modifications-forks-pull-requests-and-other-commercial-related-uses-will-be-subjected-to-copyright-violation-with-sebsequent-legal-concerns)***

⏬

### ***Please carefully read [LICENSE.md](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/LICENSE) about the Open Source restrictions and the personal use policy of this project under [GPL-3.0 license](https://www.gnu.org/licenses/gpl-3.0.en.html), any commericial uses on this project by other than the owner [@KrystalZhang612](https://github.com/KrystalZhang612) or the authorized users and organizations, including unauthorized modifications, forks, pull requests, and other commercial-related uses will be subjected to copyright violation with sebsequent legal concerns.***

# Calculator App Overview:
<pre> 
              Addition Overview:                             Subtraction Overview: 
</pre> 
<p align = "center"> 
  <img src ="https://user-images.githubusercontent.com/72481348/200421857-769879b6-b24c-4a57-977f-b30cb330fcea.mov" width="380" height="841"/>&nbsp; 
  <img src ="https://user-images.githubusercontent.com/72481348/200422241-f2319e77-0732-415b-ac4a-04a1a30781da.mov" width = "380" height ="841"/> 
</p> 
<pre> 
              Multiplication Overview:                        Division Overview: 
</pre>
<p align = "center">
  <img src ="https://user-images.githubusercontent.com/72481348/200423097-97a4b292-678b-477a-9e36-3d0f7ba5f247.mov" width="380" height="841"/>&nbsp; 
  <img src ="https://user-images.githubusercontent.com/72481348/200423193-0f72aac9-4a2a-4ac4-baec-6e315dd7fb05.mov" width="380" height="841"/>
</p>

# Build
[Method to Run & Test the Project Locally](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/README.md#method-to-run--test-the-project-locally)<br/> 
[Synchronous Developing Notes](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/README.md#synchronous-developing-notes)<br/> 
[Testing Result](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/README.md#testing-result)<br/> 
[Tags and Topics]()<br/> 
# Contribution
[Author]()
# Compatibility
|   OS             | Supported          |
| -------          | ------------------ |
| iOS 10+          | :white_check_mark: |
| < iOS 10         | :x:                |
| macOS Mojave     | ✅                 |
| macOS Monterey   | ✅                 |
# Method to Run & Test the Project Locally
### Download the entire project to local directory
### Xcode must be `13.4` and higher versions with all Xcode dependencies updated.
### Compatible with `MacOS Monterey 12.0` or higher versions
### Run the project, choose Simulator `iPhone 14` or `iPhone 14 Pro` for best compatiability.
# 🛠️  Developing Languages, Tools, and Techniques Needed
[Xcode 14.0.1 iOS 16 iPhone 14 Pro Simulator](https://developer.apple.com/documentation/xcode-release-notes/xcode-14_0_1-release-notes)<br/>
[Swift5](https://www.swift.org/blog/swift-5-released/)<br/>
[SwiftUI](https://developer.apple.com/xcode/swiftui/)<br/>
<div>
  <img src ="https://github.com/devicons/devicon/blob/master/icons/xcode/xcode-plain.svg" title ="Xcode" alt ="Xcode" width ="60" height="60"/>&nbsp;
  <img src ="https://github.com/devicons/devicon/blob/master/icons/swift/swift-original.svg"  title ="SWIFT5" alt ="SWIFT5" width ="60" height="60"/>&nbsp;
  <img src ="https://github.com/KrystalZhang612/KrystalZhang-RepliFlix/blob/main/swift%20ui%20symbol%20logo.png" title ="SwiftUI" alt ="SwiftUI" width ="60" height="60"/>
</div>

# Synchronous Developing Notes
Add IBoutlets in [ViewController.swift](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/Calculator-App/ViewController.swift):
```swift 
@IBOutlet var holder: UIView!
```
## ***Add buttons:***
Set up the zero button and make it display at the bottom center:
```swift 
 private func setupNumberPad() {
        let buttonSize = view.frame.size.width / 4
        let zeroButton = UIButton(frame: CGRect(x: 0, y:
holder.frame.size.height-buttonSize, width: buttonSize*3, height:
buttonSize))
        zeroButton.setTitleColor(.black, for: .normal)
        zeroButton.backgroundColor = .white
        zeroButton.setTitle("0", for: .normal)
        holder.addSubview(zeroButton)
}
```
[button zero displayed.PNG](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/button%20zero%20displayed.png)<br/> 
Now add 1 2 3 buttons above using a for loop:
```swift 
  for x in 0..<3 {
        let button1 = UIButton(frame: CGRect(x: buttonSize *
CGFloat(x), y: holder.frame.size.height-(buttonSize*2), width:
buttonSize, height: buttonSize))
        button1.setTitleColor(.black, for: .normal)
        button1.backgroundColor = .white
        button1.setTitle("\(x+1)", for: .normal)
        holder.addSubview(button1)
}
```



# Testing Result 
[button zero displayed.PNG](https://github.com/KrystalZhang612/KrystalZhang-Calculator-App/blob/main/button%20zero%20displayed.png)<br/> 














