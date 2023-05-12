# Verse Commons

> Common functionality that Verse is currently missing or frequently requested

## Using These Files

To use these files in your own project:

1. Open your project in UEFN
2. From the **Verse** menu choose **Verse Explorer**
3. Right-click on your project name in **Verse Explorer** and choose **Add new Verse file to project**
4. Set the name of the device to the name of the file you want to use:
    - If the file is `foo_device.verse`, name the device `foo_device`
    - If the file is `bar.verse` name the device `bar`
5. Click **Create**
6. Double-click your newly created file to open it in Visual Studio Code
7. Copy the contents of the file you want in this repository and paste it into the file in Visual Studio Code
8. Repeat steps 3 through 7 for any other files you wish to use in your project
9. Back in UEFN click on **Verse** and choose **Build Verse Code**
10. If everything compiles correctly then the functions, classes and structs defined in the files you added should now be available to your own devices and code.

## Using Array

1. Add `array.verse` to the root of your Verse project
2. Import the Array functions by putting `using { Array }` at the top of your device Verse file
3. Functions will now be available on your Array types. eg.

```
MyArray : []int = array{2, 1, 3}
MyArray.Sort(Array.Sort.orderBy.Asc, Array.Sort.CompareInts)
```

## Using Map

1. Add `map.verse` to the root of your Verse project
2. Import the Map functions by putting `using { Map }` at the top of your device Verse file
3. Functions will now be available on your Map types. eg.

```
MyMap : [string]int = map{"one" => 1, "two" => 2, "three" => 3}
MyMap.Values() # [1,2,3]
MyMap.Keys() # ["one", "two", "three"]
```