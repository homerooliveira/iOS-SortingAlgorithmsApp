![Alt text](https://i.imgur.com/SaWlE8K.png)

# Sorting Algorithms App
An open source app focused on show in a visual way how sorting algorithms actually works.

![Alt text](https://media.giphy.com/media/lSVaBYt3cXBz1bKoCV/giphy.gif)

### Do you want to contribute? Check the backlog

- [ ] New algorithms
- [ ] Control animation speed
- [ ] Enable user to add his own array
- [ ] Add algorithm description on detail scene
- [ ] Unit Tests
- [ ] More features on backlog :)

### Adding a new algorithm

Create a class implemeting the protocol ```Algorithm```. Following the example for the class ```InsertionSort```, you'd need to set the title of your algorithm, the image (pick a nice logo representing your algorithm:)) and description. In the method ```GenerateSwaps```, add the necessary logic to generate all cell swaps which would be necessary.

```Swift 
final class InsertionSort: Algorithm {
    
    final var title: String = "Insertion Sort"
    final var image: String = "ic_insertion"
    final var description: String = "Insertion Sort Description"
    
    final func generateSwaps(from list: [Int]) -> [(x0: Int, x1: Int)] {
        if list.count == 1 { return [] }
        
        var array = list
        var swaps = [(x0: Int, x1: Int)]()
        
        // APPEND ALL GENERATED SWAPS TO IT'S ARRAY
        
        return swaps
    }
}
```

### Update the data source with your new algorithm

```Swift
class AlgorithmsListPresenter {
    
    private weak var view: AlgorithmsListView?
    private let router: AlgorithmsListRoutering
    
    private let dataSource: [Algorithm] = [
        BubbleSort(),
        InsertionSort(),
        SelectionSort()
    ]
 ...
}   
```

### Submiting contributions

Try adding your own solution, feel free to suggest changes on the current code. If you're ready to submit a contribution, create a pull request describing your approach. All contributions are welcome even the small ones.

### Contributors

See you here :)
