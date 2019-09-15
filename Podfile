platform :ios, '11.0'

inhibit_all_warnings!

target 'ToDoList' do
  use_frameworks!

  #
  # unused pods
  #
  # pod 'PKHUD'
  # pod 'BulletinBoard' # v1.1 feature (onboarding tutorial)
  # pod 'Alamofire'
  # pod 'Reveal-SDK', '20', :configurations => ['Debug']
  #

  pod 'LKAlertController'
  pod 'ActionSheetPicker-3.0', :git => 'https://github.com/iPhoNewsRO/ActionSheetPicker-3.0'
  pod 'IceCream', :git => 'https://github.com/iPhoNewsRO/IceCream.git'
  pod 'UnderKeyboard'
  pod 'ActiveLabel'
  pod 'Realm'
  pod 'RealmSwift'
  pod 'RSTextViewMaster'
  pod 'AcknowList'
  pod 'BiometricAuthentication', :git => 'https://github.com/iPhoNewsRO/BiometricAuthentication'
  pod 'ImpressiveNotifications', :git => 'https://github.com/iPhoNewsRO/ImpressiveNotifications'
  pod 'Robin'
  pod 'Fabric'
  pod 'Crashlytics'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    if ['AcknowList', 'UnderKeyboard'].include? target.name
      target.build_configurations.each do |config|
        config.build_settings['SWIFT_VERSION'] = '4.2'
      end
    end
  end
end
