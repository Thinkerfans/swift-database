swift-database
==============
问题一：
CoreData: warning: Unable to load class named 'Person' for entity 'Person'.  
Class not found, using default NSManagedObject instead.

解决方案：
@objc(Person)//用Xcode自动生产Person时没有@objc(Person)这个字段，需要手动加上。
class Person: NSManagedObject {

    @NSManaged var age: NSNumber
    @NSManaged var name: String
  
}

问题二
xxx.xcdatamodeid文件的创建和Entity的创建

知识点：
1、swift数据存取
2、tableview自定义TableViewCell
3、swift对话框Alert的使用



