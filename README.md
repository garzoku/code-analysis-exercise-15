# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (person, petName){
  for (dog in person.dogs){
    if (dog.name === petName){
      return dog
    }
  }
}
```

| Input           | Output                 |
| --------------- | ---------------------- |
|`{name: "Tim", dogs: [{name:"Parker"}]}`  |`{name: "Parker"}`  | 
|`{name: "Kurt", dogs: [{name:"Flora"}]}`  |`{name: "Flora"}`    | 
|`{name: "Jane", dogs: [{name:"Pupperz"}]}`|`{name: "Pupperz"}`  | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>1). The function accepts two arguments: a person, and a pet name.<br>
2). The For-in loop iterates through every dog in dogs, with dogs being an array of objects within person.<br>
3). If there is a dog who's property of "name" matches petName, that dog's property is returned.<br>
Summary: The dogs object is nested inside of the person object. It searches through dogs for one with a property of "name" that matches petName. It then returns the object properties of the dog associated with the person.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
