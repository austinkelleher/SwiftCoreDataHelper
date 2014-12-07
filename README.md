SwiftCoreDataHelper
===================

Helper class for Core Data handling in Swift

Examples
===================

Saving a Core Data entry:

    CoreDataHelper.save("Users", dictionary: [
        "email": "a@alk.im",
        "firstName": "Austin",
        "lastName": "Kelleher"
    ])

Retreiving the first Core Data entry:

    if let user = CoreDataHelper.getFirstCoreDataResult("Users") {
      var email = user.valueForKey("email") as String
      var firstName = user.valueForKey("firstName") as String
      var lastName = user.valueForKey("lastName") as String
    }

Retreiving a specific Core Data entry by Id:

    if let user = CoreDataHelper.getCoreDataResultById("Users", id: 5) {
      var email = user.valueForKey("email") as String
      var firstName = user.valueForKey("firstName") as String
      var lastName = user.valueForKey("lastName") as String
    }
  
