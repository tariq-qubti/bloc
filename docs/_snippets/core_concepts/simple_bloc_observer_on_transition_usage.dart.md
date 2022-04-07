```dart
void main() {
  BlocOverrides.runZoned(
    () {
      return CounterBloc()
        ..add(CounterIncrementPressed())
        ..close();
    },
    blocObserver: SimpleBlocObserver(),
  );
}
```
