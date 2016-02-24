# Getting location with CLLocationManager 

First you will need to add the CLLocationManagerDelegate to your ViewController 
 ```swift
class ViewController: UIViewController, CLLocationManagerDelegate {
    var manager: CLLocationManager!
    
```

Then initialize the location manager and register as a delegate for listening to incoming location updates. 

 ```swift 
    override func viewDidLoad() {
        super.viewDidLoad()
        
        manager = CLLocationManager()
        manager.delegate = self
        manager.desiredAccuracy = kCLLocationAccuracyBest
       
        manager.requestAlwaysAuthorization()
        manager.startUpdatingLocation()
        
    }
```

The add the following delegate method to your view controller 

 ```swift 
    func locationManager(manager: CLLocationManager, didUpdateLocations locations: [CLLocation]) {
        print("locations = \(locations)")
        
        var location : CLLocationCoordinate2D = (manager.location?.coordinate)!
        
        let lat = location.latitude
        let long =  location.longitude;
        
    }
```
