A library for building REST APIs easily with Dart.

## Inspiration

Our inspiration is the simplicity of [express js][express] 👏.

[license](https://github.com/dart-lang/stagehand/blob/master/LICENSE).

## Usage

A simple usage example:

```dart
import 'package:sevr/sevr.dart';

main() {
  var serv = Sevr();

  serv.get('/test',[(req,res){
    return res.status(200).json({'status':'ok'});
  }]);
  
  serv.listen(3000,callback: (){
    print('Listening on ${3000}');
  });
}
```

## Features and bugs

Please file feature requests and bugs at the [issue tracker][tracker].

## Contributing

Fork the repo, clone and raise your pull requests against the dev branch, We look forward to your your commits! 😀

[tracker]: https://github.com/a-oboh/dart-sevr/issues
[express]: https://expressjs.com/
