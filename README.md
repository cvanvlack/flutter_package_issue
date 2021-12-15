# flutter_package_issue

Project created with
```
flutter create --project-name=flutter_package_issue --platforms=ios,android flutter_package_issue
```
updated `pubspec.yaml` to current form and got no errors.

Tried to compile for iOS and got the following error
```
Launching lib/main.dart on iPhone 13 in debug mode...
CocoaPods' output:
↳
      Preparing
    Analyzing dependencies
    Inspecting targets to integrate
      Using `ARCHS` setting to build architectures of target `Pods-Runner`: (``)
    Fetching external sources
    -> Fetching podspec for `Flutter` from `Flutter`
    -> Fetching podspec for `cloud_firestore` from `.symlinks/plugins/cloud_firestore/ios`
    cloud_firestore: Using Firebase SDK version '8.9.0' defined in 'firebase_core'
    -> Fetching podspec for `cloud_functions` from `.symlinks/plugins/cloud_functions/ios`
    cloud_functions: Using Firebase SDK version '8.9.0' defined in 'firebase_core'
    -> Fetching podspec for `firebase_auth` from `.symlinks/plugins/firebase_auth/ios`
    firebase_auth: Using Firebase SDK version '8.9.0' defined in 'firebase_core'
    -> Fetching podspec for `firebase_core` from `.symlinks/plugins/firebase_core/ios`
    firebase_core: Using Firebase SDK version '8.9.0' defined in 'firebase_core'
    -> Fetching podspec for `firebase_dynamic_links` from `.symlinks/plugins/firebase_dynamic_links/ios`
    firebase_dynamic_links: Using Firebase SDK version '8.9.0' defined in 'firebase_core'
    -> Fetching podspec for `flutter_facebook_auth` from `.symlinks/plugins/flutter_facebook_auth/ios`
    -> Fetching podspec for `google_sign_in` from `.symlinks/plugins/google_sign_in/ios`
    -> Fetching podspec for `image_picker` from `.symlinks/plugins/image_picker/ios`
    -> Fetching podspec for `integration_test` from `.symlinks/plugins/integration_test/ios`
    -> Fetching podspec for `open_mail_app` from `.symlinks/plugins/open_mail_app/ios`
    -> Fetching podspec for `path_provider_ios` from `.symlinks/plugins/path_provider_ios/ios`
    -> Fetching podspec for `share_plus` from `.symlinks/plugins/share_plus/ios`
    -> Fetching podspec for `sign_in_with_apple` from `.symlinks/plugins/sign_in_with_apple/ios`
    -> Fetching podspec for `sqflite` from `.symlinks/plugins/sqflite/ios`
    -> Fetching podspec for `url_launcher_ios` from `.symlinks/plugins/url_launcher_ios/ios`
    Resolving dependencies of `Podfile`
      CDN: trunk Relative path: CocoaPods-version.yml exists! Returning local because checking is only performed in repo update
    [!] CocoaPods could not find compatible versions for pod "cloud_firestore":
      In Podfile:
        cloud_firestore (from `.symlinks/plugins/cloud_firestore/ios`)
    Specs satisfying the `cloud_firestore (from `.symlinks/plugins/cloud_firestore/ios`)` dependency were found, but they required a higher minimum deployment target.
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:317:in `raise_error_unless_state'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:299:in `block in unwind_for_conflict'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:297:in `tap'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:297:in `unwind_for_conflict'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:682:in `attempt_to_activate'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:254:in `process_topmost_state'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:182:in `resolve'
    /Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolver.rb:43:in `resolve'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/resolver.rb:94:in `resolve'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer/analyzer.rb:1078:in `block in resolve_dependencies'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/user_interface.rb:64:in `section'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer/analyzer.rb:1076:in `resolve_dependencies'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer/analyzer.rb:124:in `analyze'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer.rb:416:in `analyze'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer.rb:241:in `block in resolve_dependencies'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/user_interface.rb:64:in `section'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer.rb:240:in `resolve_dependencies'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/installer.rb:161:in `install!'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/command/install.rb:52:in `run'
    /Library/Ruby/Gems/2.6.0/gems/claide-1.0.3/lib/claide/command.rb:334:in `run'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/lib/cocoapods/command.rb:52:in `run'
    /Library/Ruby/Gems/2.6.0/gems/cocoapods-1.11.2/bin/pod:55:in `<top (required)>'
    /usr/local/bin/pod:23:in `load'
    /usr/local/bin/pod:23:in `<main>'
Error output from CocoaPods:
↳
    [!] Automatically assigning platform `iOS` with version `9.0` on target `Runner` because no platform was specified. Please specify a platform for this target in your Podfile. See `https://guides.cocoapods.org/syntax/podfile.html#platform`.
Error running pod install
Error launching application on iPhone 13.
Exited (sigterm)
```
