# teacher

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


  Widget build(BuildContext context) {
    return Container(
      padding: const EdgeInsets.all(10.0),
      child: Column(
        children: <Widget>[
          new CheckboxListTile(
            activeColor: Colors.blue,
            title: Text('チェックボックス'),
            subtitle: Text('チェックボックスのサブタイトル'),
            secondary: new Icon(
              Icons.thumb_up,
              color: _flag ? Colors.orange[700] : Colors.grey[500],
            ),
            controlAffinity: ListTileControlAffinity.leading,
            value: _flag,
            onChanged: _handleCheckbox,
          ),
        ],
      )
    );
  }