platform :ios, '8.0'
use_frameworks!

abstract_target 'default_pods' do
    pod 'Alamofire', '~> 3.5'
    
    target 'target-Release'
    target 'target-Debug' do
        target 'target-HostTests' do
            inherit! :search_paths
        end
    end
    target 'target-Tests'
end
