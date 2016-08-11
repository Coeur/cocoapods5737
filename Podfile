platform :ios, '8.0'
use_frameworks!

abstract_target 'default_pods' do
    pod 'Alamofire', :git => 'https://github.com/Alamofire/Alamofire.git', :branch => 'swift2.3'
    
    target 'target-Release'
    target 'target-Debug'
    target 'target-Tests'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '2.3'
        end
    end
end
